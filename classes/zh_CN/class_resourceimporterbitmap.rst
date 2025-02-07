:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/4.2/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/4.2/doc/classes/ResourceImporterBitMap.xml.

.. _class_ResourceImporterBitMap:

ResourceImporterBitMap
======================

**继承：** :ref:`ResourceImporter<class_ResourceImporter>` **<** :ref:`RefCounted<class_RefCounted>` **<** :ref:`Object<class_Object>`

导入 :ref:`BitMap<class_BitMap>` 资源（布尔值的 2D 数组）。

.. rst-class:: classref-introduction-group

描述
----

:ref:`BitMap<class_BitMap>` 资源通常被用作 :ref:`TextureButton<class_TextureButton>` 和 :ref:`TouchScreenButton<class_TouchScreenButton>` 的点击遮罩。

.. rst-class:: classref-introduction-group

教程
----

- :doc:`导入图像 <../tutorials/assets_pipeline/importing_images>`

.. rst-class:: classref-reftable-group

属性
----

.. table::
   :widths: auto

   +---------------------------+-----------------------------------------------------------------------+---------+
   | :ref:`int<class_int>`     | :ref:`create_from<class_ResourceImporterBitMap_property_create_from>` | ``0``   |
   +---------------------------+-----------------------------------------------------------------------+---------+
   | :ref:`float<class_float>` | :ref:`threshold<class_ResourceImporterBitMap_property_threshold>`     | ``0.5`` |
   +---------------------------+-----------------------------------------------------------------------+---------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

属性说明
--------

.. _class_ResourceImporterBitMap_property_create_from:

.. rst-class:: classref-property

:ref:`int<class_int>` **create_from** = ``0``

用于生成位图的数据源。

\ **黑白：**\ HSV 值大于 :ref:`threshold<class_ResourceImporterBitMap_property_threshold>` 的像素将被视为“启用”（位为 ``true``\ ）。如果像素低于或等于阈值，则将被视为“禁用”（位为 ``false``\ ）。

\ **Alpha：**\ Alpha值大于 :ref:`threshold<class_ResourceImporterBitMap_property_threshold>` 的像素将被视为“启用”（位为 ``true``\ ）。如果像素低于或等于阈值，则将被视为“禁用”（位为 ``false``\ ）。

.. rst-class:: classref-item-separator

----

.. _class_ResourceImporterBitMap_property_threshold:

.. rst-class:: classref-property

:ref:`float<class_float>` **threshold** = ``0.5``

用于确定哪些位应被视为启用或禁用的阈值。另见 :ref:`create_from<class_ResourceImporterBitMap_property_create_from>`\ 。

.. |virtual| replace:: :abbr:`virtual (本方法通常需要用户覆盖才能生效。)`
.. |const| replace:: :abbr:`const (本方法没有副作用。不会修改该实例的任何成员变量。)`
.. |vararg| replace:: :abbr:`vararg (本方法除了在此处描述的参数外，还能够继续接受任意数量的参数。)`
.. |constructor| replace:: :abbr:`constructor (本方法用于构造某个类型。)`
.. |static| replace:: :abbr:`static (调用本方法无需实例，所以可以直接使用类名调用。)`
.. |operator| replace:: :abbr:`operator (本方法描述的是使用本类型作为左操作数的有效操作符。)`
.. |bitfield| replace:: :abbr:`BitField (这个值是由下列标志构成的位掩码整数。)`
