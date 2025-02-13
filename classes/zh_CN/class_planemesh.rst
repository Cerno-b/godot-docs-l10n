:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/4.2/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/4.2/doc/classes/PlaneMesh.xml.

.. _class_PlaneMesh:

PlaneMesh
=========

**继承：** :ref:`PrimitiveMesh<class_PrimitiveMesh>` **<** :ref:`Mesh<class_Mesh>` **<** :ref:`Resource<class_Resource>` **<** :ref:`RefCounted<class_RefCounted>` **<** :ref:`Object<class_Object>`

**派生：** :ref:`QuadMesh<class_QuadMesh>`

表示平面 :ref:`PrimitiveMesh<class_PrimitiveMesh>` 的类。

.. rst-class:: classref-introduction-group

描述
----

代表平面 :ref:`PrimitiveMesh<class_PrimitiveMesh>` 的类。这个扁平的网格没有厚度。默认情况下，这个网格与 X 和 Z 轴对齐；这样的旋转并不适用于公告板材质。对于公告板材质，请将 :ref:`orientation<class_PlaneMesh_property_orientation>` 改为 :ref:`FACE_Z<class_PlaneMesh_constant_FACE_Z>`\ 。

\ **注意：**\ 使用较大且有纹理的 **PlaneMesh**\ （例如地板）时，你可能在使用某些相机角度时会遇到 UV 抖动的问题。要解决这个问题，请增大 :ref:`subdivide_depth<class_PlaneMesh_property_subdivide_depth>` 和 :ref:`subdivide_width<class_PlaneMesh_property_subdivide_width>`\ ，直到无法再察觉到 UV 抖动。

.. rst-class:: classref-reftable-group

属性
----

.. table::
   :widths: auto

   +------------------------------------------------+------------------------------------------------------------------+----------------------+
   | :ref:`Vector3<class_Vector3>`                  | :ref:`center_offset<class_PlaneMesh_property_center_offset>`     | ``Vector3(0, 0, 0)`` |
   +------------------------------------------------+------------------------------------------------------------------+----------------------+
   | :ref:`Orientation<enum_PlaneMesh_Orientation>` | :ref:`orientation<class_PlaneMesh_property_orientation>`         | ``1``                |
   +------------------------------------------------+------------------------------------------------------------------+----------------------+
   | :ref:`Vector2<class_Vector2>`                  | :ref:`size<class_PlaneMesh_property_size>`                       | ``Vector2(2, 2)``    |
   +------------------------------------------------+------------------------------------------------------------------+----------------------+
   | :ref:`int<class_int>`                          | :ref:`subdivide_depth<class_PlaneMesh_property_subdivide_depth>` | ``0``                |
   +------------------------------------------------+------------------------------------------------------------------+----------------------+
   | :ref:`int<class_int>`                          | :ref:`subdivide_width<class_PlaneMesh_property_subdivide_width>` | ``0``                |
   +------------------------------------------------+------------------------------------------------------------------+----------------------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

枚举
----

.. _enum_PlaneMesh_Orientation:

.. rst-class:: classref-enumeration

enum **Orientation**:

.. _class_PlaneMesh_constant_FACE_X:

.. rst-class:: classref-enumeration-constant

:ref:`Orientation<enum_PlaneMesh_Orientation>` **FACE_X** = ``0``

**PlaneMesh** 将面向 X 轴正方向。

.. _class_PlaneMesh_constant_FACE_Y:

.. rst-class:: classref-enumeration-constant

:ref:`Orientation<enum_PlaneMesh_Orientation>` **FACE_Y** = ``1``

**PlaneMesh** 将面向 Y 轴正方向。与 Godot 3.x 中 **PlaneMesh** 的行为一致。

.. _class_PlaneMesh_constant_FACE_Z:

.. rst-class:: classref-enumeration-constant

:ref:`Orientation<enum_PlaneMesh_Orientation>` **FACE_Z** = ``2``

**PlaneMesh** 将面向 Z 轴正方向。与 Godot 3.x 中 QuadMesh 的行为一致。

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

属性说明
--------

.. _class_PlaneMesh_property_center_offset:

.. rst-class:: classref-property

:ref:`Vector3<class_Vector3>` **center_offset** = ``Vector3(0, 0, 0)``

.. rst-class:: classref-property-setget

- void **set_center_offset** **(** :ref:`Vector3<class_Vector3>` value **)**
- :ref:`Vector3<class_Vector3>` **get_center_offset** **(** **)**

生成平面的偏移量。可用于粒子。

.. rst-class:: classref-item-separator

----

.. _class_PlaneMesh_property_orientation:

.. rst-class:: classref-property

:ref:`Orientation<enum_PlaneMesh_Orientation>` **orientation** = ``1``

.. rst-class:: classref-property-setget

- void **set_orientation** **(** :ref:`Orientation<enum_PlaneMesh_Orientation>` value **)**
- :ref:`Orientation<enum_PlaneMesh_Orientation>` **get_orientation** **(** **)**

**PlaneMesh** 的朝向。可选项见 :ref:`Orientation<enum_PlaneMesh_Orientation>`\ 。

.. rst-class:: classref-item-separator

----

.. _class_PlaneMesh_property_size:

.. rst-class:: classref-property

:ref:`Vector2<class_Vector2>` **size** = ``Vector2(2, 2)``

.. rst-class:: classref-property-setget

- void **set_size** **(** :ref:`Vector2<class_Vector2>` value **)**
- :ref:`Vector2<class_Vector2>` **get_size** **(** **)**

生成平面的大小。

.. rst-class:: classref-item-separator

----

.. _class_PlaneMesh_property_subdivide_depth:

.. rst-class:: classref-property

:ref:`int<class_int>` **subdivide_depth** = ``0``

.. rst-class:: classref-property-setget

- void **set_subdivide_depth** **(** :ref:`int<class_int>` value **)**
- :ref:`int<class_int>` **get_subdivide_depth** **(** **)**

沿 Z 轴细分的次数。

.. rst-class:: classref-item-separator

----

.. _class_PlaneMesh_property_subdivide_width:

.. rst-class:: classref-property

:ref:`int<class_int>` **subdivide_width** = ``0``

.. rst-class:: classref-property-setget

- void **set_subdivide_width** **(** :ref:`int<class_int>` value **)**
- :ref:`int<class_int>` **get_subdivide_width** **(** **)**

沿 X 轴细分的次数。

.. |virtual| replace:: :abbr:`virtual (本方法通常需要用户覆盖才能生效。)`
.. |const| replace:: :abbr:`const (本方法没有副作用。不会修改该实例的任何成员变量。)`
.. |vararg| replace:: :abbr:`vararg (本方法除了在此处描述的参数外，还能够继续接受任意数量的参数。)`
.. |constructor| replace:: :abbr:`constructor (本方法用于构造某个类型。)`
.. |static| replace:: :abbr:`static (调用本方法无需实例，所以可以直接使用类名调用。)`
.. |operator| replace:: :abbr:`operator (本方法描述的是使用本类型作为左操作数的有效操作符。)`
.. |bitfield| replace:: :abbr:`BitField (这个值是由下列标志构成的位掩码整数。)`
