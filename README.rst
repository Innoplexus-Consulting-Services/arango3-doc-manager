====================
arango3-doc-manager
====================


Getting Started
===============

This package is a document manager for mongo-connector that targets
ArangoDB versions 3.x and keeps ArangoDB in sync with MongoDB.

Installation
===============

ArangoDB 3.x
-----------------

For use with an ArangoDB 3.x server, install with pip::

  pip install arango3-doc-manager

Development
-----------------

You can also install the development version of arangodb3-doc-manager manually::

  git clone https://github.com/Innoplexus-Consulting-Services/arango3-doc-manager.git

  python setup.py install

You may have to run pip with sudo, depending on where you're installing and
what privileges you have.

Running the tests::
-----------------

1. Clone the arago3-doc-manager Github repository::

  git clone https://github.com/Innoplexus-Consulting-Services/arango3-doc-manager.git

2. Go to arango3-doc-manager/tests/::

  cd arango3-doc-manager/tests/

3. Run tests::

  python test_arango3-doc-manager.py

Setting up ArangoDB Authentication
----------------------------------

ArangoDB runs with authentication by default.

Use connector_arango_auth command for below mentioned Authentication
related operations:

1. Set Auth::

  connector_arango_auth set

  source ~/.bashrc

2. Reset Auth::

  connector_arango_auth reset

  source ~/.bashrc

3. Disable Auth::

  connector_arango_auth flush

  source ~/.bashrc

Verify Auth credentials by issuing the following command on termianl:

1. Verify username::
  :~$echo $USER_ARANGO

2. Verify password::
  :~$echo $PASSWD_ARANGO

Authors
===============

1. Prashant Patil, Innoplexus
2. Suyash Masugade, Innoplexus
