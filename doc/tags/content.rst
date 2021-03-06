``content``
===========

This attribute allows to replace the content of a note with the content of a variable.

Suppose to have a variable ``foo`` with a value ``My name is John`` and the following template:

.. code-block:: xml+jinja

    <div id="pagination" t:content="foo">
        This <b>content</b> will be removed
    </div>


The output will be:

.. code-block:: xml+jinja

    <div id="pagination">My name is John</div>


This can be useful to put come "test" content in your templates that will have a nice aspect on WYSIWYG
editors, but at runtime will be replaced by real data coming from variables.
