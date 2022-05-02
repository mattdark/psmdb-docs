.. _dochome:


================================================================================
Percona Server for MongoDB |version| Documentation
================================================================================

|PSMDB| is a free, enhanced, fully compatible, source available, drop-in replacement
for MongoDB |version| Community Edition with enterprise-grade features.
It requires no changes to MongoDB applications or code.

.. hint::

   To see which version of |PSMDB| you are using check the value of the
   ``psmdbVersion`` key in the output of the `buildInfo <https://docs.mongodb.com/manual/reference/command/buildInfo/#dbcmd.buildInfo>`_ database command. If
   this key does not exist, |PSMDB| is not installed on the server.

.. rubric:: Features

|PSMDB| provides the following features:

- MongoDB's default WiredTiger_ engine
- :ref:`inmemory` storage engine
- :ref:`psmdb.data-at-rest-encryption`
- :ref:`External authentication <ext-auth>`
  using OpenLDAP or Active Directory
- :ref:`Audit logging <audit-log>`
  to track and query database interactions of users or applications
- :ref:`hot-backup` for the default WiredTiger_
- :ref:`rate-limit` to decrease the impact of the profiler on performance

To learn more about the features, available in |PSMDB|, see :ref:`compare`



.. toctree::
   :hidden:
   :caption: About Percona Server for MongoDB
   :maxdepth: 1

   Feature Comparison <comparison>

.. toctree::
   :hidden:
   :caption: Installation
   :maxdepth: 1

   install/index
   Install on Debian or Ubuntu <install/apt>
   Install on RHEL or CentOS <install/yum>
   Install from Binary Tarball <install/tarball>
   Run in a Docker Container <install/docker>
   


.. toctree::
   :hidden:
   :caption: Features
   :maxdepth: 1
   

   inmemory
   hot-backup
   rate-limit
   authentication
   authorization
   audit-logging
   log-redaction
   data-at-rest-encryption
   vault
   keyfile
   encryption-mode-switch
   kmip
   ngram-full-text-search

.. toctree::
   :hidden:
   :caption: How to
   :maxdepth: 1

   Enable authentication <enable-auth>
   Set up LDAP authentication using SASL <sasl-auth>
   Set up LDAP authentication and authorization using NativeLDAP <ldap-setup>
   x509-ldap
   kerberos
   Tune parameters <set-parameter>
   Upgrade Percona Server for MongoDB <install/upgrade-from-mongodb>
   Perform a major upgrade of Percona Server for MongoDB from 4.4 to 5.0 <install/upgrade-from-44>
   Uninstall Percona Server for MongoDB <install/uninstall>


.. toctree::
   :hidden:
   :caption: Release notes
   :maxdepth: 2

   release_notes/index


.. toctree::
   :hidden:
   :caption: Reference
   :maxdepth: 1

   contact
   glossary
   copyright
   trademark-policy

.. include:: .res/replace.txt
