Class **Phalcon\\Paginator\\Adapter\\NativeArray**
==================================================

*extends* abstract class :doc:`Phalcon\\Paginator\\Adapter <Phalcon_Paginator_Adapter>`

*implements* :doc:`Phalcon\\Paginator\\AdapterInterface <Phalcon_Paginator_AdapterInterface>`

.. role:: raw-html(raw)
   :format: html

:raw-html:`<a href="https://github.com/phalcon/cphalcon/blob/master/phalcon/paginator/adapter/nativearray.zep" class="btn btn-default btn-sm">Source on GitHub</a>`

Pagination using a PHP array as source of data

.. code-block:: php

    <?php

    use Phalcon\Paginator\Adapter\NativeArray;

    $paginator = new NativeArray(
        [
            "data"  => [
                ["id" => 1, "name" => "Artichoke"],
                ["id" => 2, "name" => "Carrots"],
                ["id" => 3, "name" => "Beet"],
                ["id" => 4, "name" => "Lettuce"],
                ["id" => 5, "name" => ""],
            ],
            "limit" => 2,
            "page"  => $currentPage,
        ]
    );



Methods
-------

public  **__construct** (*array* $config)

Phalcon\\Paginator\\Adapter\\NativeArray constructor



public  **getPaginate** ()

Returns a slice of the resultset to show in the pagination



public  **setCurrentPage** (*mixed* $page) inherited from :doc:`Phalcon\\Paginator\\Adapter <Phalcon_Paginator_Adapter>`

Set the current page number



public  **setLimit** (*mixed* $limitRows) inherited from :doc:`Phalcon\\Paginator\\Adapter <Phalcon_Paginator_Adapter>`

Set current rows limit



public  **getLimit** () inherited from :doc:`Phalcon\\Paginator\\Adapter <Phalcon_Paginator_Adapter>`

Get current rows limit



