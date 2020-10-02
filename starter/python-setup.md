# `ubuntu-python starter`
So, we have just inatalled ubuntu 20.x.
It's the current LTS version for ubuntu.
After we are successfully booted to ubuntu 20.x, as we loo through the terminal we could easily find the latest or near to the latest version of python.
So what's left to install for our python setup to be development ready.

## `mandatory`
- **`pip`**<br>
Even after the support for python2 version has been taken off, ubuntu still uses python2.x, so when installing the pip version for pip3 we need to specify the version.<br>
`sudo apt install python3-pip`<br>
Once downloaded it'll be available as PATH, hence we can call it directly from terminal anywhere in the system.<br>
`pip3 --version`<br>

## `optional`
I usually prefer :
- **`pipenv`**<br>
Python wrapper for creating and managing **virtualenvs** *(virtual environment)*. It comes really handy when managing different python project with different dependencies. Even as a beginner where you don't have that many projects to manage, it's a great practice to follow. For more we can follow official docs or this giude [here](https://realpython.com/pipenv-guide).


https://packages.ubuntu.com/
