========================================================================
Installation
========================================================================

Dependencies
============

PHPassLib requires PHP >= 5.3. Due to bugs in PHP's ``crypt()`` function
(CVE-2011-2483_ and `bug #55439`_). The library test suite is run
regularly against both PHP versions 5.3 and 5.4.

Users will also need to have the hash_ extension installed. It is
highly recommended to enable the mcrypt_ and openssl_ extensions as
well.

Installation Instructions
=========================

Using Composer
--------------

Composer_ is an easy way to manage dependencies in your PHP projects.
The PHP Password Library can be found in the default Packagist_
repository.

After installing Composer into your project, the PHP Password Library
can be installed by adding the following lines to your ``composer.json``
file and running the Composer command line tool:

.. code-block:: json

    {
      "require": {
        "rych/phpass": "3.0.*"
      }
    }

Using PEAR
----------

Installing via PEAR is a simple matter of discovering the PEAR channel
and installing the rych/PHPassLib package.

.. code-block:: bash

    pear channel-discover rchouinard.github.com/pear
    pear install rych/PHPassLib

.. _CVE-2011-2483: https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2011-2483
.. _`bug #55439`: https://bugs.php.net/bug.php?id=55439
.. _hash: http://php.net/manual/en/book.hash.php
.. _mcrypt: http://php.net/manual/en/book.mcrypt.php
.. _openssl: http://php.net/manual/en/book.openssl.php
.. _Composer: http://getcomposer.org/
.. _Packagist: http://packagist.org/
