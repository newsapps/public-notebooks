Tribune DataViz Public Notebooks
================================

Assumptions
-----------

* Python >= 3.4 (Some of the older notebooks may only work with 2.7, but I want to use Python 3 moving forward)
* virtualenvwrapper

Installation
------------

Clone the repository:

    https://github.com/newsapps/public-notebooks.git

Create a virtualenv:

    mkvirtualenv public-notebooks

Install dependencies:

    cd public-notebooks
    workon public-notebooks
    pip install -r requirements.txt

Avoid leaking credentials
-------------------------

Some of these notebooks, particularly those dealing with crime stats, pull data from NewsroomDB.  While security measures prevent outside access, we should avoid leaking the URLs of internal resources.  Your notebooks should pull things like credentials or URLs from environment variables instead of hard-coding them in the scripts.

