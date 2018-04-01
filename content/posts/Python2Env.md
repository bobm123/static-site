Title: Working on Legacy Python
Date: 2018-03-02 12:40
Modified: 2018-04-02 12:40
Status: published
Category: Programming
Tags: python2, legacy python, programming
Slug: environment-for-legacy-python
Authors: Bob Marchese
Summary: Makign an environment for working with legacy python

You've moved on to Python 3 by now right? Well even so, you might still need to run legacy python occasionally. Maybe you're bringing some olde code up to date and also need to install a specifig version of some package to go with it. So you can't just use the system python delivered with Ubuntu LTS or old redhat install because that might break something. This, in my opinion is a good job for virtual environments.

Here's what I do. Simply make a virtual environment called 'legacy' and switch to that when needed. The '-p' flag lets you specify a specific version of python to use. For example, on my Win10 lappy I did this using windows virtual environment wrapper:
```
d:\ancient_scripts>mkvirtualenv legacy -p d:\Python27\python.exe
Running virtualenv with interpreter d:\Python27\python.exe
New python executable in D:\Envs\legacy\Scripts\python.exe
Installing setuptools, pip, wheel...done.

d:\ancient_scripts>workon legacy
(legacy) d:\ancient_scripts>
```
