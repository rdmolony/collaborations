# From Excel to Python via Ploomber

This short article is relevant to you if ...

- Your data is too large for `Microsoft Excel`
- You seek more reproduciblity & automation (downloading, wrangling, saving data)
- You are willing to put in the time to learn a few new `Python` based tools

---

My team & I wanted to model the Dublin energy system for the purposes of energy planning.

Previously, we solely used `Microsoft Excel`.  It's a powerful tool and fast to learn, however, it can be limiting.  Large data sets can cause crashes, and sharing analytics when the underlying data is closed-access is hard because data and logic (cleaning, merging data etc) tend to be tightly coupled.  This coupling makes it difficult for others to reproduce, reuse or improve your analytics. 

`Python` enables decoupling of data and logic, however, the switch is no easy feat.  You first need to learn the basics of `Python` and the `pandas` "extension" (dependency) for spreadsheet operations.  Next, you'll need some tool to run your scripts (like `Jupyter Notebook`).  If you have trouble installing everything, you may have no choice but to use the command line.  If you want to share your work, you'll also need to specify the versions of your dependencies using a configuration file.  This is a lot to ask.

Once you start using `Jupyter Notebook` the temptation is to write all of your logic in a single notebook.  In time as this notebook grows, it becomes more difficult to maintain, run and share.  To simplify maintenance and speed up runtimes, you can split notebooks into smaller components (scripts or notebooks).  Now a new challenge, how to run them?  

We used the `ploomber` library as it uses a simple configuration file (`yaml`) to specify file run-order.  You can now read, edit & run flows without reading any code.  As an added bonus, `ploomber` enables rendering flow steps as notebooks that can be run independently of the flow.  Now another problem, how to share this work with colleagues without requiring them to install anything? 

We used `GitHub` is for storing & versioning code, `Amazon s3` for data storage, and `binder.org` to create a sandbox environment that anyone can run in their browser.  `GitHub` uses `Git` to version code, which if used directly can be hard to get your head around.  Graphics User Interfaces (GUI) like `Git Graph` for `Vscode` or `Github Desktop` help.  `Amazon s3` enables sharing data via URLs, or if it's closed-access, programatically via credentials.

And that's it, if you think the cost of upskilling is worth the benefits checkout the `GitHub` repository to view, run or copy any of our projects:

https://github.com/codema-dev/projects

![Tools.drawio.svg](Tools.drawio.svg)
