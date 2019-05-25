[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/meli-lewis/nw_news_nerds/master)

# Data Exploration with Python

This repository contains code and datasets to facilitate a workshop on using Python for data exploration, including steps for data acquisition, cleaning and normalization. We'll be using a subset of the Washington State Patrol data on traffic stops from the [Stanford Open Policing Project](https://openpolicing.stanford.edu/data/), as the full dataset is 1.5GB and may not play nice with the service we'll be using for the class. Also, as of this writing, GitHub does not by default allow file sizes greater than 100MB.

## Getting Started

For the Northwest News Nerds 2019 workshop, you need simply visit [this mybinder.org link](https://mybinder.org/v2/gh/meli-lewis/nw_news_nerds/master)!

### If you want this code to run locally

If you're already a Python 3 user comfortable with virtual environments, you can skip these directions, create a new virtual environment for the class, and run `pip install -r requirements.txt` to jump in.

#### 1: Get this repo on your machine.

  - If you'd like to use Git to do so, continue with these directions.
  - If not, select ![Clone or Download](b.png) and choose "Download ZIP." Unzip the file, taking note of where it was downloaded, and skip to [2: Ensure you have Python 3](#2-ensure-you-have-python-3).

1. Check that Git is installed:
    ```bash
    which git
    ```
   - If installed, this will return a path (e.g., `/usr/local/bin/git`)
   - If it's not installed, [GitHub's directions](https://help.github.com/articles/set-up-git/#setting-up-git) for downloading and setting it up are helpful.

2. Select ![Clone or Download](b.png) and use the clipboard icon to make sure you grab the full URL for this repo. GitHub's [directions for this](https://help.github.com/articles/cloning-a-repository/) are good too!

#### 2: Ensure you have Python 3.

  1. Check that Python 3 is installed:
    ```bash
    which python3
    ```
    - If it's installed, it should return a path (e.g., `/usr/local/bin/python3`).
    - If it's not installed, you can download it from [python.org](https://www.python.org/downloads/)

#### 3. Set up a virtual environment

**Creation** | You can put your virtual environment in any directory, but if you're new to working with them, it may be easiest to put it in the same directory as this code.

  - [Here](https://docs.python.org/3/library/venv.html#creating-virtual-environments) are the docs on creating virtual environments, but if you're comfortable, you can use one of the following commands.

      - If you're using a Linux or Mac OS:
  ```bash
     python3 -m venv /path/to/new/virtual/environment
  ```
      - If you're using a Windows OS:
  ```
    c:\>c:\Python35\python -m venv c:\path\to\myenv
  ```

**Activation** | Here there's some more variation. You can find the following table in the virtual environment documentation, but I'm including it here for convenience.

| Platform | Shell      | Command                         |
|----------|------------|---------------------------------|
| Posix    | bash/zsh   | `$ source /bin/activate`        |
|          | fish       | `$ . /bin/activate.fish`        |
|          | csh/tcsh   | `$ source /bin/activate.csh`    |
| Windows  | cmd.exe    | `C:\> \Scripts\activate.bat`    |
|          | PowerShell | `PS C:\> \Scripts\Activate.ps1` |

You'll know that it's activated if you see its name in parentheses prepended to your command prompt, like this:

```bash
(virtual_env_name) my-computer $
```

It can be hard to understand at first, but this virtual environment will remain activated no matter which directory you move to, so you don't have to worry about where you are when you activate it. To exit, you can run

```bash
deactivate
```

#### 4. Install the packages for the workshop

*With the virtual environment activated*, install the packages used for this workshop with the Python package management tool `pip`.

Some of you may already know the drill; some others may only ever have used `pip` to install packages on the command line, e.g. `pip install pandas`. Still others may not have used it before, and that's okay!

```bash
   pip install -r requirements.txt
```

You should then see a lot printed to your screen, starting with `Collecting beautifulsoup4>=4.7.1 (from -r requirements.txt (line 1))
`

#### 5. Run the notebook

You have two options here!

1. The class will write code together using `practice-notebook.ipynb`.
2. You'll also have the option of reading and playing around with complete code in `reference_notebook.ipynb`.

Either way, if you're not using `mybinder.org`, you'll want to navigate to whichever directory you want to use and run
```bash
jupyter notebook
```

## But most importantly

If you're trying to set this up and running into problems, try not to feel discouraged! This is a complex process and will not be necessary for the class. However, you're also welcome to ask for help through [PyLadies Portland](https://www.meetup.com/PyLadies-PDX/) or by [contacting me directly](http://melidata.com/contact).
