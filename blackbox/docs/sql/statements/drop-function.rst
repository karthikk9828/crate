.. highlight:: psql
.. _ref-drop-function:

=================
``DROP FUNCTION``
=================

Drop a function.

.. rubric:: Table of Contents

.. contents::
   :local:

Synopsis
========

::

    DROP FUNCTION [ IF EXISTS ] function_name
        ( [ [ arg_name ] arg_type [, ...] ] )

Description
===========

``DROP FUNCTION`` drops a function. A function name and argument types must be
specified.

Parameters
==========

:IF EXISTS:
  Do not produce an error if the function doesn't exist.

:function_name:
  The name of the function to drop.

:arg_name:
  The name given to an argument.

  Function arguments do not retain names, but you can name them in your
  query for documentation purposes. Note that ``DROP FUNCTION`` will
  ignore argument names, since only the argument data types are needed
  to identify the function.

:arg_type:
  The data type of an argument, if any.

  See :ref:`data-types` for more information about the supported types.
