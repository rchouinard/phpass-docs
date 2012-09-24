========================================================================
PHP Password Library |release| Documentation
========================================================================

Introduction
============

The PHP Password Library (PHPassLib) is a library for PHP 5.3+ designed
to make working with passwords as easy as possible. Tasks such as
creating password hashes, verifying passwords, and migrating stored
hashes are made simple.

.. code-block:: php

    <?php
    require 'PHPassLib.php';
    use PHPassLib\Hash\BCrypt;
    
    $hash = BCrypt::hash($password);
    if (BCrypt::verify($password, $hash)) {
        // Authentication passed!
    }

Overview
========

 * :doc:`install`

Indices and tables
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`
