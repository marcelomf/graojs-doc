graojs-doc
==========

[graoJS](http://graojs.org) Docs

You can access all versions of this documentation in [http:\\docs.graojs.org].

Building
--------

First, install [Sphinx-Pocoo](http://sphinx-doc.org/) and [Sphinx Bootstrap Theme](https://github.com/ryan-roemer/sphinx-bootstrap-theme):

~~~bsh
apt-get install python-setuptools python-dev build-essential
easy_install -U Sphinx
pip install sphinx_bootstrap_theme
~~~

Now, clone or download the docs source:

~~~bsh
git clone https://github.com/synackbr/graojs-doc.git
~~~

~~~bsh
wget https://github.com/synackbr/graojs-doc.git/tarball/master -O graojs-docs.tar.gz
tar xzf graojs-doc.tar.gz
~~~

Now, get into `graojs-doc` directory and choose what language you want to build,
doing a `source` symbolic link to the desired language (`en` on the example):

~~~bsh
rm source
ln -sf en source
~~~

Now you can build:

~~~bsh
make html
~~~

Other formats supported by Sphinx-Pocoo has not been tested for a while.