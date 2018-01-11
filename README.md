# Python in the Georgetown Data Science Program

As part of Georgetown University's [Data Science Certificate program](http://scs.georgetown.edu/programs/375/data-science/), the faculty have created a series of in-class and supplementary labs to help reinforce the lecture topics. The labs should be run in [Python 3.6](https://docs.python.org/3/whatsnew/3.6.html) and predominantly use [Jupyter Notebook](http://jupyter.org/) for execution.

## Computer Setup
**Students are responsible for software installation and maintenance of their computers.** The faculty and teaching assistants will be able to help students with some troubleshooting; however, none of the faculty uses Windows as a programming environment or with any type of regularity. We will do our best to assist students with any issues but request that you please follow the installation instructions written below.

## Python Prerequisite

As noted in the prerequisites for this program, students are expected to have familiarity with Python. In addition, they should be able to navigate their system from the command line. Students who can successfully work on the command line and have an understanding of Python generally find the lab work less frustrating.

If you not familiar with working at the command line to perform tasks, such as changing directories or launching programs, there are multiple free or low-cost online resources and tutorials. Some examples include:

* [Command Line Crash Course](http://cli.learncodethehardway.org/book/)
* [Introduction to Shell for Data Science](https://www.datacamp.com/courses/introduction-to-shell-for-data-science)
* [UNIX Tutorial for Beginners](http://www.ee.surrey.ac.uk/Teaching/Unix/)

### Python Installation

Please note that in this course we will be exclusively using Python 3. Experienced Python users should feel free to use whatever setup works for them. However, regardless of OS, students are highly encouraged to take advantage of the [Anaconda](https://www.continuum.io/) distribution and look into the use of [environments](https://conda.io/docs/user-guide/tasks/manage-environments.html).

The latest version of Python available for download can be found [here](https://www.python.org/downloads/). For further details on the installation process, please refer to the [documentation](https://docs.python.org/3/using/index.html).

### Anaconda
Students are encouraged to install Python via the Anaconda distribution since it includes a pre-configured collection of the most commonly used packages they'll encounter throughout the program, such as `matplotlib`, `numpy`, `pandas`, and `scikit-learn`.

* [Download](https://www.anaconda.com/download/) the installer appropriate for your OS.

Once installed, use Anaconda's package manager, Conda, to verify that you have the most current updates. A package manager is an important tool that automates the process of installing, updating, and removing packages.

`conda update conda`<br/>
`conda update anaconda`

While Anaconda takes care of compiler dependencies for common packages, we recommend students install the `scipy` package while setting up Anaconda since it should be installed before packages that they will need later on in the course, such as `Seaborn`. It can be installed with following command:

`conda install scipy`<br />

## Git
Git is a free and open source distributed version control system that allows multiple users to track file changes and coordinate their work.
* [Download](https://git-scm.com/downloads) and [install](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) Git. We will not use any of the GUIs in class.
* [Configure](https://git-scm.com/book/en/v2/Getting-Started-First-Time-Git-Setup) Git
* Prerequisite: students should already have a [GitHub](https://github.com/) account. If not, set one up now.

Students that are new to Git or who are looking to refresh their skills are encouraged to work through the following tutorials or any other resources they find helpful.
* [Git and GitHub](https://www.datacamp.com/courses/introduction-to-git-for-data-science)
* [Try Git](https://try.github.io/)

### Jupyter Notebook

[Jupyter Notebook](http://jupyter.org/) is a web application that allows users to create and share documents containing live code, text, and visualizations. A majority of the labs are in Jupyter Notebook, so it is vital that students know how to work with them. You are highly encouraged to complete this [tutorial](https://www.datacamp.com/community/tutorials/tutorial-jupyter-notebook) if you are new to Jupyter Notebook or need to refresh your skills.

To install Jupyter using pip:  `pip install jupyter`

To install Jupyter using conda:  `conda install jupyter`

Once installed, launch a notebook by running the following command in your Terminal(Mac and Linux)/Command Prompt (Windows):

`jupyter notebook`

For additional information on running Jupyter Notebooks, please read the [documentation](https://jupyter.readthedocs.io/en/latest/running.html#running).

### Python Packages

One item students will encounter as throughout the labs is the `requirements.txt` file. This file lists the packages required for run the lab and can also be used by pip to install packages. To install packages with a requirements file, use the following command:

`pip install -r requirements.txt`

Students that installed Python via Anaconda should run the following code:

`conda install --yes --file requirements.txt`

**Please note:** The dependencies listed in the `requirements.txt` file are intended to set the entire Python environment, so if you have a different version of a library already installed, pip will overwrite it! Therefore, the faculty highly encourages students to use environments.

## Lab Workflow

In-class labs will generally begin by following this workflow:

* [Clone a GitHub repository](https://help.github.com/articles/cloning-a-repository/)
* Navigate to the repository on your computer
* Launch a Jupyter Notebook

Try it now with this repository! In the upper right-hand part of the page, you'll find the green **Clone or download** button. When clicked, you'll have the option to copy the repository's clone URL.

Next, open your terminal and navigate to the directory where you want to clone the repository. The following code includes the URL and will clone this repo on your computer:

`git clone https://github.com/georgetown-analytics/XBUS-500-01.Foundations-of-Data-Analytics-and-Data-Science.git`<br/>

*If you encounter issues cloning a repository in-class, verify you are on SaxaNet, not GuestNet.*

Next, perform a directory listing. You should now see a directory called `XBUS-500-01.Foundations-of-Data-Analytics-and-Data-Science`. Change into that directory.

`cd XBUS-500-01.Foundations-of-Data-Analytics-and-Data-Science`

Now if you do a directory listing, you should see the following items. However, if you are on Windows and do not see the files that start with '.' you may need to [adjust your settings](http://www.howtogeek.com/howto/windows-vista/show-hidden-files-and-folders-in-windows-vista/).

	.gitignore
	LICENSE
	README.md
	welcome.ipynb

Next, we will launch Jupyter Notebook. There are a few options you can use, but to get started we recommend using one of the following commands:

`jupyter notebook`

Or to launch a specific notebook:

`jupyter notebook welcome.ipynb`

## General Troubleshooting Tip

When you are having issues—Google. It is unlikely you are the only one encountering errors and [Stack Overflow](http://stackoverflow.com/) is full of solutions. Including your OS and "python" in your search with the error message will help you find the most useful results. For example: `python windows install scipy <error message>`
