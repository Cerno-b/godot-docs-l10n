:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/4.2/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/4.2/doc/classes/PackedColorArray.xml.

.. _class_PackedColorArray:

PackedColorArray
================

:ref:`Color<class_Color>` 紧缩数组。

.. rst-class:: classref-introduction-group

描述
----

专门设计用于存放 :ref:`Color<class_Color>` 的数组。数据是紧密存放的，因此能够在数组较大时节省内存。

.. note::

	通过 C# 使用这个 API 时有显著的不同。详见 :ref:`doc_c_sharp_differences`\ 。

.. rst-class:: classref-reftable-group

构造函数
--------

.. table::
   :widths: auto

   +-------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`PackedColorArray<class_PackedColorArray>` | :ref:`PackedColorArray<class_PackedColorArray_constructor_PackedColorArray>` **(** **)**                                                      |
   +-------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`PackedColorArray<class_PackedColorArray>` | :ref:`PackedColorArray<class_PackedColorArray_constructor_PackedColorArray>` **(** :ref:`PackedColorArray<class_PackedColorArray>` from **)** |
   +-------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`PackedColorArray<class_PackedColorArray>` | :ref:`PackedColorArray<class_PackedColorArray_constructor_PackedColorArray>` **(** :ref:`Array<class_Array>` from **)**                       |
   +-------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------+

.. rst-class:: classref-reftable-group

方法
----

.. table::
   :widths: auto

   +-------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>`                         | :ref:`append<class_PackedColorArray_method_append>` **(** :ref:`Color<class_Color>` value **)**                                         |
   +-------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------+
   | void                                            | :ref:`append_array<class_PackedColorArray_method_append_array>` **(** :ref:`PackedColorArray<class_PackedColorArray>` array **)**       |
   +-------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`int<class_int>`                           | :ref:`bsearch<class_PackedColorArray_method_bsearch>` **(** :ref:`Color<class_Color>` value, :ref:`bool<class_bool>` before=true **)**  |
   +-------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------+
   | void                                            | :ref:`clear<class_PackedColorArray_method_clear>` **(** **)**                                                                           |
   +-------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`int<class_int>`                           | :ref:`count<class_PackedColorArray_method_count>` **(** :ref:`Color<class_Color>` value **)** |const|                                   |
   +-------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`PackedColorArray<class_PackedColorArray>` | :ref:`duplicate<class_PackedColorArray_method_duplicate>` **(** **)**                                                                   |
   +-------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------+
   | void                                            | :ref:`fill<class_PackedColorArray_method_fill>` **(** :ref:`Color<class_Color>` value **)**                                             |
   +-------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`int<class_int>`                           | :ref:`find<class_PackedColorArray_method_find>` **(** :ref:`Color<class_Color>` value, :ref:`int<class_int>` from=0 **)** |const|       |
   +-------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>`                         | :ref:`has<class_PackedColorArray_method_has>` **(** :ref:`Color<class_Color>` value **)** |const|                                       |
   +-------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`int<class_int>`                           | :ref:`insert<class_PackedColorArray_method_insert>` **(** :ref:`int<class_int>` at_index, :ref:`Color<class_Color>` value **)**         |
   +-------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>`                         | :ref:`is_empty<class_PackedColorArray_method_is_empty>` **(** **)** |const|                                                             |
   +-------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>`                         | :ref:`push_back<class_PackedColorArray_method_push_back>` **(** :ref:`Color<class_Color>` value **)**                                   |
   +-------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------+
   | void                                            | :ref:`remove_at<class_PackedColorArray_method_remove_at>` **(** :ref:`int<class_int>` index **)**                                       |
   +-------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`int<class_int>`                           | :ref:`resize<class_PackedColorArray_method_resize>` **(** :ref:`int<class_int>` new_size **)**                                          |
   +-------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------+
   | void                                            | :ref:`reverse<class_PackedColorArray_method_reverse>` **(** **)**                                                                       |
   +-------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`int<class_int>`                           | :ref:`rfind<class_PackedColorArray_method_rfind>` **(** :ref:`Color<class_Color>` value, :ref:`int<class_int>` from=-1 **)** |const|    |
   +-------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------+
   | void                                            | :ref:`set<class_PackedColorArray_method_set>` **(** :ref:`int<class_int>` index, :ref:`Color<class_Color>` value **)**                  |
   +-------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`int<class_int>`                           | :ref:`size<class_PackedColorArray_method_size>` **(** **)** |const|                                                                     |
   +-------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`PackedColorArray<class_PackedColorArray>` | :ref:`slice<class_PackedColorArray_method_slice>` **(** :ref:`int<class_int>` begin, :ref:`int<class_int>` end=2147483647 **)** |const| |
   +-------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------+
   | void                                            | :ref:`sort<class_PackedColorArray_method_sort>` **(** **)**                                                                             |
   +-------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`PackedByteArray<class_PackedByteArray>`   | :ref:`to_byte_array<class_PackedColorArray_method_to_byte_array>` **(** **)** |const|                                                   |
   +-------------------------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------+

.. rst-class:: classref-reftable-group

操作符
------

.. table::
   :widths: auto

   +-------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>`                         | :ref:`operator !=<class_PackedColorArray_operator_neq_PackedColorArray>` **(** :ref:`PackedColorArray<class_PackedColorArray>` right **)** |
   +-------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`PackedColorArray<class_PackedColorArray>` | :ref:`operator +<class_PackedColorArray_operator_sum_PackedColorArray>` **(** :ref:`PackedColorArray<class_PackedColorArray>` right **)**  |
   +-------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>`                         | :ref:`operator ==<class_PackedColorArray_operator_eq_PackedColorArray>` **(** :ref:`PackedColorArray<class_PackedColorArray>` right **)**  |
   +-------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Color<class_Color>`                       | :ref:`operator []<class_PackedColorArray_operator_idx_int>` **(** :ref:`int<class_int>` index **)**                                        |
   +-------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

构造函数说明
------------

.. _class_PackedColorArray_constructor_PackedColorArray:

.. rst-class:: classref-constructor

:ref:`PackedColorArray<class_PackedColorArray>` **PackedColorArray** **(** **)**

构造空的 **PackedColorArray**\ 。

.. rst-class:: classref-item-separator

----

.. rst-class:: classref-constructor

:ref:`PackedColorArray<class_PackedColorArray>` **PackedColorArray** **(** :ref:`PackedColorArray<class_PackedColorArray>` from **)**

构造给定 **PackedColorArray** 的副本。

.. rst-class:: classref-item-separator

----

.. rst-class:: classref-constructor

:ref:`PackedColorArray<class_PackedColorArray>` **PackedColorArray** **(** :ref:`Array<class_Array>` from **)**

构造新的 **PackedColorArray**\ 。你也可以传一个通用 :ref:`Array<class_Array>` 进行转换。

\ **注意：**\ 使用元素初始化 **PackedColorArray** 时，必须使用元素为 :ref:`Color<class_Color>` 的 :ref:`Array<class_Array>`\ ：

::

    var array = PackedColorArray([Color(0.1, 0.2, 0.3), Color(0.4, 0.5, 0.6)])

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

方法说明
--------

.. _class_PackedColorArray_method_append:

.. rst-class:: classref-method

:ref:`bool<class_bool>` **append** **(** :ref:`Color<class_Color>` value **)**

向数组末尾追加一个元素（\ :ref:`push_back<class_PackedColorArray_method_push_back>` 的别名）。

.. rst-class:: classref-item-separator

----

.. _class_PackedColorArray_method_append_array:

.. rst-class:: classref-method

void **append_array** **(** :ref:`PackedColorArray<class_PackedColorArray>` array **)**

在该数组的末尾追加一个 **PackedColorArray**\ 。

.. rst-class:: classref-item-separator

----

.. _class_PackedColorArray_method_bsearch:

.. rst-class:: classref-method

:ref:`int<class_int>` **bsearch** **(** :ref:`Color<class_Color>` value, :ref:`bool<class_bool>` before=true **)**

使用二进法查找已有值的索引（如果该值尚未存在于数组中，则为保持排序顺序的插入索引）。传递 ``before`` 说明符是可选的。如果该参数为 ``false``\ ，则返回的索引位于数组中该值的所有已有的条目之后。

\ **注意：**\ 在未排序的数组上调用 :ref:`bsearch<class_PackedColorArray_method_bsearch>` 会产生预料之外的行为。

.. rst-class:: classref-item-separator

----

.. _class_PackedColorArray_method_clear:

.. rst-class:: classref-method

void **clear** **(** **)**

清空数组。相当于调用 :ref:`resize<class_PackedColorArray_method_resize>` 时指定大小为 ``0``\ 。

.. rst-class:: classref-item-separator

----

.. _class_PackedColorArray_method_count:

.. rst-class:: classref-method

:ref:`int<class_int>` **count** **(** :ref:`Color<class_Color>` value **)** |const|

返回元素在数组中出现的次数。

.. rst-class:: classref-item-separator

----

.. _class_PackedColorArray_method_duplicate:

.. rst-class:: classref-method

:ref:`PackedColorArray<class_PackedColorArray>` **duplicate** **(** **)**

创建该数组的副本，并将该副本返回。

.. rst-class:: classref-item-separator

----

.. _class_PackedColorArray_method_fill:

.. rst-class:: classref-method

void **fill** **(** :ref:`Color<class_Color>` value **)**

将数组中的所有元素都设为给定的值。通常与 :ref:`resize<class_PackedColorArray_method_resize>` 一起使用，创建给定大小的数组并初始化元素。

.. rst-class:: classref-item-separator

----

.. _class_PackedColorArray_method_find:

.. rst-class:: classref-method

:ref:`int<class_int>` **find** **(** :ref:`Color<class_Color>` value, :ref:`int<class_int>` from=0 **)** |const|

在数组中搜索值并返回其索引，如果未找到则返回 ``-1`` 。可选地，可以传递起始搜索索引。

.. rst-class:: classref-item-separator

----

.. _class_PackedColorArray_method_has:

.. rst-class:: classref-method

:ref:`bool<class_bool>` **has** **(** :ref:`Color<class_Color>` value **)** |const|

如果该数组包含 ``value``\ ，则返回 ``true``\ 。

.. rst-class:: classref-item-separator

----

.. _class_PackedColorArray_method_insert:

.. rst-class:: classref-method

:ref:`int<class_int>` **insert** **(** :ref:`int<class_int>` at_index, :ref:`Color<class_Color>` value **)**

在数组中给定的位置插入一个新元素。这个位置必须是有效的，或者是在数组的末端（\ ``idx == size()``\ ）。

.. rst-class:: classref-item-separator

----

.. _class_PackedColorArray_method_is_empty:

.. rst-class:: classref-method

:ref:`bool<class_bool>` **is_empty** **(** **)** |const|

该数组为空时，返回 ``true``\ 。

.. rst-class:: classref-item-separator

----

.. _class_PackedColorArray_method_push_back:

.. rst-class:: classref-method

:ref:`bool<class_bool>` **push_back** **(** :ref:`Color<class_Color>` value **)**

将一个值添加到数组中。

.. rst-class:: classref-item-separator

----

.. _class_PackedColorArray_method_remove_at:

.. rst-class:: classref-method

void **remove_at** **(** :ref:`int<class_int>` index **)**

从数组中删除位于索引的元素。

.. rst-class:: classref-item-separator

----

.. _class_PackedColorArray_method_resize:

.. rst-class:: classref-method

:ref:`int<class_int>` **resize** **(** :ref:`int<class_int>` new_size **)**

设置数组的大小。如果数组被增大，则保留数组末端的元素。如果数组被缩小，则将数组截断到新的大小。

.. rst-class:: classref-item-separator

----

.. _class_PackedColorArray_method_reverse:

.. rst-class:: classref-method

void **reverse** **(** **)**

将数组中的元素逆序排列。

.. rst-class:: classref-item-separator

----

.. _class_PackedColorArray_method_rfind:

.. rst-class:: classref-method

:ref:`int<class_int>` **rfind** **(** :ref:`Color<class_Color>` value, :ref:`int<class_int>` from=-1 **)** |const|

逆序搜索数组。还可以传递起始搜索位置索引。如果为负，则起始索引被视为相对于数组的结尾。

.. rst-class:: classref-item-separator

----

.. _class_PackedColorArray_method_set:

.. rst-class:: classref-method

void **set** **(** :ref:`int<class_int>` index, :ref:`Color<class_Color>` value **)**

更改给定索引处的 :ref:`Color<class_Color>`\ 。

.. rst-class:: classref-item-separator

----

.. _class_PackedColorArray_method_size:

.. rst-class:: classref-method

:ref:`int<class_int>` **size** **(** **)** |const|

返回数组中元素的个数。

.. rst-class:: classref-item-separator

----

.. _class_PackedColorArray_method_slice:

.. rst-class:: classref-method

:ref:`PackedColorArray<class_PackedColorArray>` **slice** **(** :ref:`int<class_int>` begin, :ref:`int<class_int>` end=2147483647 **)** |const|

返回该 **PackedColorArray** 的切片，是从 ``begin``\ （含）到 ``end``\ （不含）的全新 **PackedColorArray**\ 。

\ ``begin`` 和 ``end`` 的绝对值会按数组大小进行限制，所以 ``end`` 的默认值会切到数组大小为止（即 ``arr.slice(1)`` 是 ``arr.slice(1, arr.size())`` 的简写）。

如果 ``begin`` 或 ``end`` 为负，则表示相对于数组的末尾（即 ``arr.slice(0, -2)`` 是 ``arr.slice(0, arr.size() - 2)`` 的简写）。

.. rst-class:: classref-item-separator

----

.. _class_PackedColorArray_method_sort:

.. rst-class:: classref-method

void **sort** **(** **)**

将该数组中的元素按升序排列。

.. rst-class:: classref-item-separator

----

.. _class_PackedColorArray_method_to_byte_array:

.. rst-class:: classref-method

:ref:`PackedByteArray<class_PackedByteArray>` **to_byte_array** **(** **)** |const|

返回 :ref:`PackedByteArray<class_PackedByteArray>`\ ，每个颜色都被编码为字节。

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

操作符说明
----------

.. _class_PackedColorArray_operator_neq_PackedColorArray:

.. rst-class:: classref-operator

:ref:`bool<class_bool>` **operator !=** **(** :ref:`PackedColorArray<class_PackedColorArray>` right **)**

如果数组内容不同，则返回 ``true``\ 。

.. rst-class:: classref-item-separator

----

.. _class_PackedColorArray_operator_sum_PackedColorArray:

.. rst-class:: classref-operator

:ref:`PackedColorArray<class_PackedColorArray>` **operator +** **(** :ref:`PackedColorArray<class_PackedColorArray>` right **)**

返回新的 **PackedColorArray**\ ，新数组的内容为此数组在末尾加上 ``right``\ 。为了提高性能，请考虑改用 :ref:`append_array<class_PackedColorArray_method_append_array>`\ 。

.. rst-class:: classref-item-separator

----

.. _class_PackedColorArray_operator_eq_PackedColorArray:

.. rst-class:: classref-operator

:ref:`bool<class_bool>` **operator ==** **(** :ref:`PackedColorArray<class_PackedColorArray>` right **)**

如果两个数组的内容相同，即对应索引号的 :ref:`Color<class_Color>` 相等，则返回 ``true``\ 。

.. rst-class:: classref-item-separator

----

.. _class_PackedColorArray_operator_idx_int:

.. rst-class:: classref-operator

:ref:`Color<class_Color>` **operator []** **(** :ref:`int<class_int>` index **)**

返回索引 ``index`` 处的\ :ref:`Color<class_Color>`\ 。负数索引可以从末端开始访问元素。使用超出数组范围的索引将导致出错。

.. |virtual| replace:: :abbr:`virtual (本方法通常需要用户覆盖才能生效。)`
.. |const| replace:: :abbr:`const (本方法没有副作用。不会修改该实例的任何成员变量。)`
.. |vararg| replace:: :abbr:`vararg (本方法除了在此处描述的参数外，还能够继续接受任意数量的参数。)`
.. |constructor| replace:: :abbr:`constructor (本方法用于构造某个类型。)`
.. |static| replace:: :abbr:`static (调用本方法无需实例，所以可以直接使用类名调用。)`
.. |operator| replace:: :abbr:`operator (本方法描述的是使用本类型作为左操作数的有效操作符。)`
.. |bitfield| replace:: :abbr:`BitField (这个值是由下列标志构成的位掩码整数。)`
