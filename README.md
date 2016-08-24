# Python in the Georgetown Data Science Program


As part of the [Data Science Certificate at Georgetown](http://scs.georgetown.edu/programs/375/data-science/) we have created labs for the classes to help reinforce lecture topics. Staring with the Fall 2016 term, all labs will be run in [Python 3.5](https://docs.python.org/3/index.html) and predominantly use [Jupyter Notebook](http://jupyter.org/) for execution. 

Students are responsible for software installation and maintenance of their computers. The faculty will be able to assist with some troubleshooting but please note- no one currently on the faculty uses Windows as a programming environment or with any type of regularity. We will do our best to assist Windows users with any issues but request that you please follow the installation instructions as written below. We have recently tested this setup on Windows 10 and know the labs we currently run will work with these instructions. 


## Python Prerequisite

As noted in the prerequisites for this program, you are expected to have familiarity with Python. We also expect you to be able to navigate your system from the command line. Students who can successfully work on the command line and have and understanding of python generally find the lab work less frustrating. If you are not familiar with working on the command line to perform tasks such as changing directories or launching programs, there are multiple free online resources and tutorials. Some examples include:

* [Command Line Crash Course](http://cli.learncodethehardway.org/book/)
* [PowerShell](https://onedrive.live.com/view.aspx?resid=5A8D2641E0963A97!6929&ithint=file%2cpdf&app=WordPdf&authkey=!AJdUaNzW7L9yC18)
* [OS X/ *nix](http://www.ee.surrey.ac.uk/Teaching/Unix/)

We encourage you to take advantage of the [Anaconda](https://www.continuum.io/) distribution (regardless of OS) and look at the use of environments.

**If you are a Windows user:** our install instructions below **require** you to use Anaconda. Frequently used Python packages in data science, most notably [SciPy](https://www.scipy.org/), [NumPy](http://www.numpy.org/), and  [Matplotlib](http://matplotlib.org/), requires building both C and Fortran extensions which most Windows machines do not have the compiler for. Using Anaconda solves this problem for you.

## Jupyter Notebook

"[The Jupyter Notebook](http://jupyter.org/) is a web application that allows you to create and share documents that contain live code, equations, visualizations and explanatory text. Uses include: data cleaning and transformation, numerical simulation, statistical modeling, machine learning and much more."[^1] A majority of labs are in Jupyter Notebook. There is an overview of the lab workflow below where you will learn to launch them. You are highly encouraged to go through the [tutorial](https://jupyter-notebook-beginner-guide.readthedocs.io/en/latest/what_is_jupyter.html) available online.

##Installation

The information below gets you started on the installation of Anaconda, Git, and some packages we will use. Experienced Python users should feel free to use whatever setup works for them. Windows users should follow these instructions as written because we know they work. We expect you to be comfortable installing packages as needed and to do so for the labs. 

### General troubleshooting tip

If you run into an issue installing a program with pip, try conda if it is available to you (i.e. you are using Anaconda). (OS X users will also have to use homebrew for our MongoDB lab so you can try that as well.) If you still have issues, search google. It is unlikely you are the only one encountering errors and [stackoverflow](http://stackoverflow.com/) is full of solutions. Including your OS and "python" in your google search with the error message will help you get the results you are looking for. For example- "python windows install scipy <error message>"

### Anaconda

* [Download](https://www.continuum.io/downloads) and install Anaconda
* Verify you have the current updates:<br />
```conda update conda```<br />
```conda update anaconda```
* Optional: [create an environment](http://conda.pydata.org/docs/using/envs.html)

### Git

* [Download](https://git-scm.com/downloads) and [install](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) Git (We do not use any of the GUIs in class)
* [Configure](https://git-scm.com/book/en/v2/Getting-Started-First-Time-Git-Setup) Git
* Prerequisite: you should already have a [GitHub](https://github.com/) account. If not, set one up now.

### Jupyter

Jupyter is available through your package installer- i.e. ```pip install jupyter``` and/ or ```conda install jupyter```

### Python Packages

As we have seen above, packages can be installed via the use of a package manager like pip, conda, or homebrew.

One item you will encounter as we go through labs is the "requirements.txt" file. This file will list the packages required for the lab and can also be used by pip to install packages. To install packages with a requirements file, you use the following command:

```pip install -r requirements.txt```

***This section is for Windows users.*** As noted above, Anaconda takes care of compiler dependencies for common packages. There is one other "gotcha" we have encountered. You need to install scipy with conda (**DO NOT** use pip) and before you install seaborn. It is recommended to do this while setting up Anaconda so you are ready to go when the time comes. Execute the following command:<br />
```conda install scipy```<br />

## Lab Workflow

Lab portions of the class generally follow this workflow:

* Clone a repository from GitHub
* Navigate to the repository on your system
* Launch a Jupyter notebook

Try it now with this repository.

First, open your terminal program. Navigate to the location where you would like to clone the repository. When you clone a repository, you will automatically create a new directory that is named for the repository you are cloning.

```git clone https://github.com/georgetown-analytics/XBUS-500-01.Foundations-of-Data-Analytics-and-Data-Science.git```<br />

If you encounter issues cloning the repository, verify you are on SaxaNet, not GuestNet.

(If you are already familiar with Git and Github, you are welcome to follow your own workflow. We will have a Git lab in the Software Engineering class if you have not worked with it before.)

Perform a directory listing. You should now see a directory called "XBUS-500-01.Foundations-of-Data-Analytics-and-Data-Science". Change into that directory.

```cd XBUS-500-01.Foundations-of-Data-Analytics-and-Data-Science```

If you do a directory listing now, you should see the following items:

	.gitignore
	LICENSE
	README.md
	welcome.ipynb
	
If you are on windows and do not see the files that start with '.' you may need to [adjust your settings](http://www.howtogeek.com/howto/windows-vista/show-hidden-files-and-folders-in-windows-vista/).

Now we will launch the notebook. There are a few options you can use, but to get started today we recommend one of the following. You can either launch the server which will give you a dashboard in your web browser:

```jupyter notebook``` <br />

Or launch a specific notebook:

```jupyter notebook welcome.ipynb``` <br />

[^1]: http://jupyter.org/











