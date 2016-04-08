---
layout: workshop
sort: 5
title: "Apache Spark"
image: "spark-logo.png"
repo: "https://github.com/dsiufl/Python-Workshops"
summary: > 
  Introduction to text mining with the <a href="http://spark.apache.org/">Apache Spark</a> 
  computation engine using Python and Juypiter notebooks.

---
Open-sourced less than 2 years ago, Spark is on track to overtake Hadoop in popularity and flexibility as a distributed computation engine. According to the [2016 stackoverflow Developer Survey](http://stackoverflow.com/research/developer-survey-2016#technology-top-paying-tech),
Spark (and Scala which is the programming language most used with Spark) are the top paying software development technologies.

## Workshop Outline

In this workshop we explain what Spark is and how it works. Then we will describe the basics of running Spark on your computer and programming for it through an iPython notebook. We will write some Python to perform text mining with Spark on a small dataset. At the end of the workshop we will demonstrate running the same code distributed across a cluster with a much larger dataset to show how Spark parallelizes and distributes computation.

The dataset for this workshop will be made available at the workshop.

## Software Configuration

For this workshop we will be installing Spark locally on everyone's laptops
so you can run it whenever you want. Spark requires Java as well. We will 
be programming with Python 2.7 in Jupyter notebooks so we will need to
connect the Python interpreter run by the notebook to the Spark engine.

Please complete the following setup sections and make sure the check at the
end of each section works for you.

### Installing Java

1. Download the [Java SE development kit](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html)
   for your operating system.
1. Run the installer and accept the defaults except do **not** install the Ask
   Toolbar if prompted to do so.

#### Check It!

On Windows open a Command Prompt or on OS X open a Terminal and type `java 
-version`. You should see something that starts with `java version "1.8.0_77"`.
   
### Installing Spark

1. On OS X, download the [Spark tarball](http://spark.apache.org/downloads.html) from the Spark site.
   Select version 1.6.1, "Pre-built for Hadoop 2.6 and later", and "Select Apache Mirror".
   You can then click on the file named "spark-1.6.1-bin-hadoop2.6.tgz" which is a link that
   will take you to a page with a link to the download. The file will now probably be in your Downloads directory.
1. **OR** On Windows, you can download the same file as above but re-compressed to a [.zip from a
   DSI web server here](http://python.acis.ufl.edu/spark-1.6.1-bin-hadoop2.6.zip).
   The file will now probably be in your Downloads directory.
1. Open a Command Prompt in Windows or a Terminal on OS X.
1. Create a directory for this workshop on your Desktop.
1. Extract the tarball or zip file to the new directory you just created so it
   looks like this when using the Command Prompt or Terminal
   
   <img src="{{ site.baseurl }}/img/workshops/spark_desktop_dir.png" />
   
1. Change to the `spark-1.6.1-bin-hadoop2.6\bin` sub directory.
1. On Windows run `pyspark.cmd` or on OS X run `./pyspark`
1. On Windows, if you have a window pop up that says Windows Firewall has 
   blocked Java, click Allow Access.
1. You should now see something that looks like:

   <img src="{{ site.baseurl }}/img/workshops/spark_pyspark.png" />
   
1. Press Ctl-D to exit pyspark.

   
#### Check It!

If the steps above worked, everything should be fine.


### Installing Python and Jupyter notebooks

1. Download the [Anaconda Python 2.7 installer](https://www.continuum.io/downloads)
   for your operating system.
1. When installing, you can use the defaults but make sure the "Add Anaconda to my PATH"
   option is checked.
   
#### Check it!
On Windows open a Command Prompt or on OS X open a Terminal and type
```python --version
```
You should see something like 
```Python 2.7.11 :: Anaconda 4.0.0 (64-bit)
```

To make sure notebooks are working, type `jupyter notebook`. You should have a
browser window come up with the jupyter notebook interface in it. To exit, 
close the browser window and press Ctl-C in the Terminal window to shut down
the notebook server.

### Starting a notebook with Spark

For today's workshop, we are going to just use some boilerplate code at the top
of our notebook to start Spark. It is possible to configure Jupyter to start a
Spark context for you however be aware that Jupyter and iPython notebooks [are
different things](http://blog.jupyter.org/2015/04/15/the-big-split/) and you
will find a lot of how-tos on the internet about configuring iPython but none
about Jupyter.

1. Download the [Spark_Workshop_Notebook.ipynb](https://raw.githubusercontent.com/dsiufl/Spark-Workshop/master/Spark_Workshop_Notebook.ipynb) 
by right-clicking on that link and choosing "Save as File".
1. Move the Spark_Workshop_Notebook.ipynb to the Spark Workshop directory you 
   created earlier.
1. Open a Command Prompt in Windows or Terminal in OS X and change to the Spark
   Workshop directory.
1. Run `jupyter notebook`.
1. In the browser window that opens, click on the Spark_Workshop_Notebook.ipynb
   file to open it.
1. Edit the variable `spark_home` to be the **full** path to the directory that
   contains the extracted Spark programs.
1. Run the cells and make sure you get no errors.

<img src="{{ site.baseurl }}/img/workshops/spark_notebook.png" />


## Now you're ready to start learning Spark!