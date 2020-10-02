# `ubuntu-python starter`
So, we have just inatalled ubuntu 20.x.
It's the current LTS version for ubuntu.
After we are successfully booted to ubuntu 20.x, as we loo through the terminal we could easily find the latest or near to the latest version of python.
So what's left to install for our python setup to be development ready.

## `mandatory`
### `pip`<br>
Even after the support for python2 version has been taken off, ubuntu still uses python2.x, so when installing the pip version for pip3 we need to specify the version.<br>
`sudo apt install python3-pip`<br>

Once downloaded it'll be available as PATH, hence we can call it directly from terminal anywhere in the system. Remember to use **`pip3`** insted of `pip`.<br>
`pip3 --version`<br>

## `optional`
I usually prefer :
### `pipenv`<br>
Python wrapper for creating and managing **virtualenvs** *(virtual environment)*. It comes really handy when managing different python project with different dependencies.<br>
Even as a beginner where you don't have that many projects to manage, it's a great practice to follow.<br>
For more we can follow official docs or this gude [here](https://realpython.com/pipenv-guide).
**steps to setup pipenv in ubuntu**<br>
`pip3 install pipenv --user`<br>

Now we have installed `pipenv` as python3 package and we can access **pipenv** using `python3 -m pipenv <command>`, it's not that hard to remember thing but we can make it work just by `pipenv install`.<br>
- **Add `pipenv` directory path to PATH**<br>
1. open terminal in `/home` directory<br>
2. `ls -a` should provide all the available files in the home directory, we need to edit `.profile`<br>
3. `sudo gedit .profile`, this will open `.profile` in editor with user permissions.<br>
4. At the very end of file on a newline, add `export PATH="<dir-path>:$PATH"` where <**dir-path**> should be replaced with the path to your binary folder where pipenv is contained usually `/home/<user-name>/.local/bin` (can be obtained when installing *pipenv* as WARNING).<br>
5. To refresh the new path variables, type `source .profile` or logoff, then logon.<br>
Now PATH to pipenv is successfully added, that means we can use `pipenv` directly. Test by `pipenv --version`. <br>


https://packages.ubuntu.com/
