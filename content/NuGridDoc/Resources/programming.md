# Essential Skills for NuGrid Members and Users

## Unix command line
NuGrid users need to have a basic grasp of the Linux command line.

* [Essential aspects and further resources](./command_line.md)

## General programming
NuGrid is about nuclear astrophysics simulations which requires building codes which requires programming. The following is a list of possible places to start learning about programming:

1. [Newman: Computational Physics _with Python_](http://www-personal.umich.edu/~mejn/computational-physics) (Some chapters are online)
2. [Stickler & Schachinger: Basic Concepts in Computational Physics](http://voyager.library.uvic.ca/vwebv/holdingsInfo?bibId=3086030) (available as ebook from the UVic library)
3. [Langtangen: A Primer on Scientific Programming with Python](http://voyager.library.uvic.ca/vwebv/holdingsInfo?searchId=4972&recCount=25&recPointer=13&bibId=2865846) (available as ebook from the UVic library)
4. [Roundy: Introduction to Computational Physics](http://www.lulu.com/ca/en/shop/david-roundy/introduction-to-computational-physics/ebook/product-17437845.html) (free ebook)
5. [Cunningham: Python in 24 hours](http://voyager.library.uvic.ca/vwebv/holdingsInfo?searchId=5015&recCount=25&recPointer=17&bibId=3208444) (available as ebook from the UVic library)
6. [Pierro: Annotated Algorithms in Python](https://books.google.ca/books/about/Annotated_Algorithms_in_Python.html?id=cZyPngEACAAJ&redir_esc=y)
7. Specifically for numerical work there is the classic text [Press et al.: Numerical Recipes](http://www.nr.com)



## Python

* [Learn python](http://www.learnpython.org)
* [codeacademy.org](https://www.codecademy.com/learn/python) 
* [PHYS248 2nd year class at UVic](https://github.com/fherwig/physmath248_pilot)
* [NuGridPy](https://github.com/NuGrid/NuGridPy)

We recommend the [Anaconda](https://www.continuum.io/downloads) python distribution. It comes with its own package manager [conda](http://conda.pydata.org/docs/py2or3.html#create-python-2-or-3-environments) which makes [setting up virtual environments](http://conda.pydata.org/docs/using/envs.html) very easy. These virtual environment allow you to load different versions of packages. This is especially useful if you would like to try your code with both [python 2.7 and 3.5](http://conda.pydata.org/docs/py2or3.html#create-python-2-or-3-environments).

If you have used pip and virtualenv in the past, then [conda does the job of both of these](http://conda.pydata.org/docs/_downloads/conda-pip-virtualenv-translator.html).


### Quicklinks
* [Managing environments](http://conda.pydata.org/docs/using/envs.html)

### Common commands 
Here are some examples how to used conda, go to the [original conda documentation](http://conda.pydata.org/docs/using/index.html) for up-to-date and detailed info:

command | comment
--------------|-------------------
`source activate snowflakes` | activate environment snowflakes
`conda info --envs`   | list all environments
 `conda env export` | Export environment, list packages available in this environment
`conda create -n myenv python=2 numpy` |   create python 2 environment with name _myenv_ and install the  numpy  packages 

