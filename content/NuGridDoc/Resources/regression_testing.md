# Regression Testing

This page explains the general schema behind the NuGrid regression test suite(s). For information on the
regression testing of a specific NuGrid module (e.g. NuGridPy), see that repository's wiki page. 

## Travis CI

NuGrid uses a continuous integration (CI) service called Travis CI to do most of its regression testing. 
Travis allows a broad range of test packages, called builds, to be run remotely and automatically, triggered via changes 
(such as a commit or pull request) to NuGrid's GitHub repositories. 

### Logging in

To access the Travis CI build pages, as well as to see the status of particular Travis builds integrated into
the GitHub page, simply [log in to Travis with GitHub](https://travis-ci.org/). If you still can't see any repositories
or integration on the GitHub page, your NuGrid membership may be set to private. To solve this, go to the [NuGrid users page](https://github.com/orgs/NuGrid/people) and find yourself, then toggle "Private" to "Public." It may take some time for the Travis CI page to sync with your GitHub account. 

### Writing a Travis script

Travis communicates with GitHub repositories using the `.travis.yml` script. Any branch of any repository which contains
such a script will automatically be detected in the **My Repositories** section of the Travis CI webpage. 
These scripts can contain a host of instructions, including `install` to install dependencies, `notifications`
to display the results of testing, and `script` to which any command line executable instructions can be given.
The documentation (including tutorials) for writing these Travis scripts can be found [here](https://docs.travis-ci.com/).

### Running the tests

The `travis.yml` scripts will execute automatically whenever a commit or pull request is made to the repository that they
live in. The triggering of this can be customized on the Travis CI webpage. Once the build is complete and has passed 
or failed, notifications can take the form of e-mails, Slack posts, etc. (again, this is customizable within 
the script itself). 

In addition, so long as you have logged into Travis via GitHub, your GitHub page should have the build status of a given
commit or pull request embedded right into it (see image below):

![Failed Travis build](http://i.imgur.com/diGJmIh.png)

The red "X" to the right of this pull request indicates that whatever changes are being made have caused the regression
tests to fail! Note that **even when GitHub says it can go ahead with the merge, the regression tests can still fail** 
which means the changes in your commit or pull request have broken the code. 

## Jupyter (iPython) Notebooks

A number of NuGrid examples and tests also take the form of interactive Jupyter notebooks. These can be useful
for manually testing things like plotting functionality; however, it is the current view of the NuGrid collaboration 
that the core regression testing be done in a way that minimizes required user input and upkeep. These notebooks can 
thus also be converted directly to python scripts using the `nbconvert` command and then executed, all of which can
easily be written into a `travis.yml` script.

## Building a test package

What form a regression test package takes will depend on what NuGrid module you are testing. For instance, 
NuGridPy testing is done using `.py` python scripts, with python packages such as `unittest` providing the
test structure. If you would like to know how to go about building or modifying a given test platform, it
would be best to look at the wiki page for the repository of interest.
