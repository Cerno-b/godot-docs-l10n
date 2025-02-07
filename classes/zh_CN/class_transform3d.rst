:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/4.2/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/4.2/doc/classes/Transform3D.xml.

.. _class_Transform3D:

Transform3D
===========

代表 3D 变换的 3×4 矩阵。

.. rst-class:: classref-introduction-group

描述
----

用于 3D 线性变换的 3×4 矩阵（3 行 4 列），可以表示平移、旋转、缩放等变换，由 :ref:`basis<class_Transform3D_property_basis>`\ （前三列）和 :ref:`origin<class_Transform3D_property_origin>` 的 :ref:`Vector3<class_Vector3>`\ （最后一列）组成。

更多信息请阅读文档文章《矩阵与变换》。

.. note::

	通过 C# 使用这个 API 时有显著的不同。详见 :ref:`doc_c_sharp_differences`\ 。

.. rst-class:: classref-introduction-group

教程
----

- :doc:`数学文档索引 <../tutorials/math/index>`

- :doc:`矩阵与变换 <../tutorials/math/matrices_and_transforms>`

- :doc:`使用 3D 变换 <../tutorials/3d/using_transforms>`

- `矩阵变换演示 <https://godotengine.org/asset-library/asset/584>`__

- `3D 平台跳跃演示 <https://godotengine.org/asset-library/asset/125>`__

- `2.5D 演示 <https://godotengine.org/asset-library/asset/583>`__

.. rst-class:: classref-reftable-group

属性
----

.. table::
   :widths: auto

   +-------------------------------+--------------------------------------------------+--------------------------------------+
   | :ref:`Basis<class_Basis>`     | :ref:`basis<class_Transform3D_property_basis>`   | ``Basis(1, 0, 0, 0, 1, 0, 0, 0, 1)`` |
   +-------------------------------+--------------------------------------------------+--------------------------------------+
   | :ref:`Vector3<class_Vector3>` | :ref:`origin<class_Transform3D_property_origin>` | ``Vector3(0, 0, 0)``                 |
   +-------------------------------+--------------------------------------------------+--------------------------------------+

.. rst-class:: classref-reftable-group

构造函数
--------

.. table::
   :widths: auto

   +---------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Transform3D<class_Transform3D>` | :ref:`Transform3D<class_Transform3D_constructor_Transform3D>` **(** **)**                                                                                                                                                        |
   +---------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Transform3D<class_Transform3D>` | :ref:`Transform3D<class_Transform3D_constructor_Transform3D>` **(** :ref:`Transform3D<class_Transform3D>` from **)**                                                                                                             |
   +---------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Transform3D<class_Transform3D>` | :ref:`Transform3D<class_Transform3D_constructor_Transform3D>` **(** :ref:`Basis<class_Basis>` basis, :ref:`Vector3<class_Vector3>` origin **)**                                                                                  |
   +---------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Transform3D<class_Transform3D>` | :ref:`Transform3D<class_Transform3D_constructor_Transform3D>` **(** :ref:`Projection<class_Projection>` from **)**                                                                                                               |
   +---------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Transform3D<class_Transform3D>` | :ref:`Transform3D<class_Transform3D_constructor_Transform3D>` **(** :ref:`Vector3<class_Vector3>` x_axis, :ref:`Vector3<class_Vector3>` y_axis, :ref:`Vector3<class_Vector3>` z_axis, :ref:`Vector3<class_Vector3>` origin **)** |
   +---------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

.. rst-class:: classref-reftable-group

方法
----

.. table::
   :widths: auto

   +---------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Transform3D<class_Transform3D>` | :ref:`affine_inverse<class_Transform3D_method_affine_inverse>` **(** **)** |const|                                                                                                                                |
   +---------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Transform3D<class_Transform3D>` | :ref:`interpolate_with<class_Transform3D_method_interpolate_with>` **(** :ref:`Transform3D<class_Transform3D>` xform, :ref:`float<class_float>` weight **)** |const|                                              |
   +---------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Transform3D<class_Transform3D>` | :ref:`inverse<class_Transform3D_method_inverse>` **(** **)** |const|                                                                                                                                              |
   +---------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>`               | :ref:`is_equal_approx<class_Transform3D_method_is_equal_approx>` **(** :ref:`Transform3D<class_Transform3D>` xform **)** |const|                                                                                  |
   +---------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>`               | :ref:`is_finite<class_Transform3D_method_is_finite>` **(** **)** |const|                                                                                                                                          |
   +---------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Transform3D<class_Transform3D>` | :ref:`looking_at<class_Transform3D_method_looking_at>` **(** :ref:`Vector3<class_Vector3>` target, :ref:`Vector3<class_Vector3>` up=Vector3(0, 1, 0), :ref:`bool<class_bool>` use_model_front=false **)** |const| |
   +---------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Transform3D<class_Transform3D>` | :ref:`orthonormalized<class_Transform3D_method_orthonormalized>` **(** **)** |const|                                                                                                                              |
   +---------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Transform3D<class_Transform3D>` | :ref:`rotated<class_Transform3D_method_rotated>` **(** :ref:`Vector3<class_Vector3>` axis, :ref:`float<class_float>` angle **)** |const|                                                                          |
   +---------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Transform3D<class_Transform3D>` | :ref:`rotated_local<class_Transform3D_method_rotated_local>` **(** :ref:`Vector3<class_Vector3>` axis, :ref:`float<class_float>` angle **)** |const|                                                              |
   +---------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Transform3D<class_Transform3D>` | :ref:`scaled<class_Transform3D_method_scaled>` **(** :ref:`Vector3<class_Vector3>` scale **)** |const|                                                                                                            |
   +---------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Transform3D<class_Transform3D>` | :ref:`scaled_local<class_Transform3D_method_scaled_local>` **(** :ref:`Vector3<class_Vector3>` scale **)** |const|                                                                                                |
   +---------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Transform3D<class_Transform3D>` | :ref:`translated<class_Transform3D_method_translated>` **(** :ref:`Vector3<class_Vector3>` offset **)** |const|                                                                                                   |
   +---------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Transform3D<class_Transform3D>` | :ref:`translated_local<class_Transform3D_method_translated_local>` **(** :ref:`Vector3<class_Vector3>` offset **)** |const|                                                                                       |
   +---------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

.. rst-class:: classref-reftable-group

操作符
------

.. table::
   :widths: auto

   +-----------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>`                             | :ref:`operator !=<class_Transform3D_operator_neq_Transform3D>` **(** :ref:`Transform3D<class_Transform3D>` right **)**                     |
   +-----------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`AABB<class_AABB>`                             | :ref:`operator *<class_Transform3D_operator_mul_AABB>` **(** :ref:`AABB<class_AABB>` right **)**                                           |
   +-----------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`PackedVector3Array<class_PackedVector3Array>` | :ref:`operator *<class_Transform3D_operator_mul_PackedVector3Array>` **(** :ref:`PackedVector3Array<class_PackedVector3Array>` right **)** |
   +-----------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Plane<class_Plane>`                           | :ref:`operator *<class_Transform3D_operator_mul_Plane>` **(** :ref:`Plane<class_Plane>` right **)**                                        |
   +-----------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Transform3D<class_Transform3D>`               | :ref:`operator *<class_Transform3D_operator_mul_Transform3D>` **(** :ref:`Transform3D<class_Transform3D>` right **)**                      |
   +-----------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Vector3<class_Vector3>`                       | :ref:`operator *<class_Transform3D_operator_mul_Vector3>` **(** :ref:`Vector3<class_Vector3>` right **)**                                  |
   +-----------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Transform3D<class_Transform3D>`               | :ref:`operator *<class_Transform3D_operator_mul_float>` **(** :ref:`float<class_float>` right **)**                                        |
   +-----------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Transform3D<class_Transform3D>`               | :ref:`operator *<class_Transform3D_operator_mul_int>` **(** :ref:`int<class_int>` right **)**                                              |
   +-----------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>`                             | :ref:`operator ==<class_Transform3D_operator_eq_Transform3D>` **(** :ref:`Transform3D<class_Transform3D>` right **)**                      |
   +-----------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

常量
----

.. _class_Transform3D_constant_IDENTITY:

.. rst-class:: classref-constant

**IDENTITY** = ``Transform3D(1, 0, 0, 0, 1, 0, 0, 0, 1, 0, 0, 0)``

没有应用平移、旋转、缩放的 **Transform3D**\ 。当应用于其他数据结构时，\ :ref:`IDENTITY<class_Transform3D_constant_IDENTITY>` 不执行变换。

.. _class_Transform3D_constant_FLIP_X:

.. rst-class:: classref-constant

**FLIP_X** = ``Transform3D(-1, 0, 0, 0, 1, 0, 0, 0, 1, 0, 0, 0)``

应用了垂直于 YZ 平面镜像操作的 **Transform3D**\ 。

.. _class_Transform3D_constant_FLIP_Y:

.. rst-class:: classref-constant

**FLIP_Y** = ``Transform3D(1, 0, 0, 0, -1, 0, 0, 0, 1, 0, 0, 0)``

应用了垂直于 XZ 平面镜像操作的 **Transform3D**\ 。

.. _class_Transform3D_constant_FLIP_Z:

.. rst-class:: classref-constant

**FLIP_Z** = ``Transform3D(1, 0, 0, 0, 1, 0, 0, 0, -1, 0, 0, 0)``

应用了垂直于 XY 平面镜像操作的 **Transform3D**\ 。

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

属性说明
--------

.. _class_Transform3D_property_basis:

.. rst-class:: classref-property

:ref:`Basis<class_Basis>` **basis** = ``Basis(1, 0, 0, 0, 1, 0, 0, 0, 1)``

基是一个矩阵，包含 3 个 :ref:`Vector3<class_Vector3>` 作为其列：X 轴、Y 轴、Z 轴。这些向量可以被解释为随物体移动的局部坐标系的基向量。

.. rst-class:: classref-item-separator

----

.. _class_Transform3D_property_origin:

.. rst-class:: classref-property

:ref:`Vector3<class_Vector3>` **origin** = ``Vector3(0, 0, 0)``

变换的平移偏移量，即第 3、4 列。相当于数组索引 ``3``\ 。

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

构造函数说明
------------

.. _class_Transform3D_constructor_Transform3D:

.. rst-class:: classref-constructor

:ref:`Transform3D<class_Transform3D>` **Transform3D** **(** **)**

构造默认初始化为 :ref:`IDENTITY<class_Transform3D_constant_IDENTITY>` 的 **Transform3D**\ 。

.. rst-class:: classref-item-separator

----

.. rst-class:: classref-constructor

:ref:`Transform3D<class_Transform3D>` **Transform3D** **(** :ref:`Transform3D<class_Transform3D>` from **)**

构造给定 **Transform3D** 的副本。

.. rst-class:: classref-item-separator

----

.. rst-class:: classref-constructor

:ref:`Transform3D<class_Transform3D>` **Transform3D** **(** :ref:`Basis<class_Basis>` basis, :ref:`Vector3<class_Vector3>` origin **)**

从 :ref:`Basis<class_Basis>` 和 :ref:`Vector3<class_Vector3>` 构造 Transform3D。

.. rst-class:: classref-item-separator

----

.. rst-class:: classref-constructor

:ref:`Transform3D<class_Transform3D>` **Transform3D** **(** :ref:`Projection<class_Projection>` from **)**

通过修剪投影矩阵的最后一行，从 :ref:`Projection<class_Projection>` 中构造 Transform3D（不会复制 ``from.x.w``\ 、\ ``from.y.w``\ 、\ ``from.z.w``\ 、\ ``from.w.w``\ ）。

.. rst-class:: classref-item-separator

----

.. rst-class:: classref-constructor

:ref:`Transform3D<class_Transform3D>` **Transform3D** **(** :ref:`Vector3<class_Vector3>` x_axis, :ref:`Vector3<class_Vector3>` y_axis, :ref:`Vector3<class_Vector3>` z_axis, :ref:`Vector3<class_Vector3>` origin **)**

从四个 :ref:`Vector3<class_Vector3>` 值（矩阵列）构造 Transform3D。每个轴对应于局部基向量（其中一些可能已被缩放）。

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

方法说明
--------

.. _class_Transform3D_method_affine_inverse:

.. rst-class:: classref-method

:ref:`Transform3D<class_Transform3D>` **affine_inverse** **(** **)** |const|

假设该基可逆（必须具有非零行列式），返回该变换的逆。

.. rst-class:: classref-item-separator

----

.. _class_Transform3D_method_interpolate_with:

.. rst-class:: classref-method

:ref:`Transform3D<class_Transform3D>` **interpolate_with** **(** :ref:`Transform3D<class_Transform3D>` xform, :ref:`float<class_float>` weight **)** |const|

返回将该变换与其他变换使用给定权重 ``weight`` 进行插值的结果（权重范围为 0.0 到 1.0）。

.. rst-class:: classref-item-separator

----

.. _class_Transform3D_method_inverse:

.. rst-class:: classref-method

:ref:`Transform3D<class_Transform3D>` **inverse** **(** **)** |const|

返回变换的逆，假设该变换的基是正交的（即旋转/反射可以，缩放/倾斜不行）。使用 :ref:`affine_inverse<class_Transform3D_method_affine_inverse>` 进行非正交变换（例如缩放）。

.. rst-class:: classref-item-separator

----

.. _class_Transform3D_method_is_equal_approx:

.. rst-class:: classref-method

:ref:`bool<class_bool>` **is_equal_approx** **(** :ref:`Transform3D<class_Transform3D>` xform **)** |const|

如果通过在每个分量上运行 :ref:`@GlobalScope.is_equal_approx<class_@GlobalScope_method_is_equal_approx>`\ ，该变换和 ``xform`` 近似相等，则返回 ``true``\ 。

.. rst-class:: classref-item-separator

----

.. _class_Transform3D_method_is_finite:

.. rst-class:: classref-method

:ref:`bool<class_bool>` **is_finite** **(** **)** |const|

如果该变换是有限的，则返回 ``true``\ ，判断方法是在每个分量上调用 :ref:`@GlobalScope.is_finite<class_@GlobalScope_method_is_finite>`\ 。

.. rst-class:: classref-item-separator

----

.. _class_Transform3D_method_looking_at:

.. rst-class:: classref-method

:ref:`Transform3D<class_Transform3D>` **looking_at** **(** :ref:`Vector3<class_Vector3>` target, :ref:`Vector3<class_Vector3>` up=Vector3(0, 1, 0), :ref:`bool<class_bool>` use_model_front=false **)** |const|

返回该变换经过旋转后的副本，此时向前的轴（-Z）指向 ``target`` 的位置。

向上的轴（+Y）在保持与向前的轴垂直的前提下，尽可能接近 ``up`` 向量。最终的变换是标准正交变换。变换中原有的旋转、缩放、偏斜信息会被丢弃。\ ``target`` 和 ``up`` 向量不能为零，不能互相平行，使用全局/父级空间。

如果 ``use_model_front`` 为 ``true``\ ，则会将 +Z 轴（资产正面）作为向前的轴（此时 +X 为左），指向 ``target`` 的位置。默认情况下会将 -Z 轴（相机前方）作为向前的轴（此时 +X 为右）。

.. rst-class:: classref-item-separator

----

.. _class_Transform3D_method_orthonormalized:

.. rst-class:: classref-method

:ref:`Transform3D<class_Transform3D>` **orthonormalized** **(** **)** |const|

返回使用正交基（90 度）以及归一化的轴向量（缩放为 1 或 -1）的变换。

.. rst-class:: classref-item-separator

----

.. _class_Transform3D_method_rotated:

.. rst-class:: classref-method

:ref:`Transform3D<class_Transform3D>` **rotated** **(** :ref:`Vector3<class_Vector3>` axis, :ref:`float<class_float>` angle **)** |const|

返回该变换的副本，该副本围绕给定的 ``axis`` 轴进行了夹角为 ``angle`` 的旋转操作（单位为弧度）。

\ ``axis`` 必须为归一化的向量。

这个方法的结果和让 ``X`` 变换与相应的旋转变换 ``R`` 从左侧相乘一致，即 ``R * X``\ ，但进行了优化。

可以视作在全局/父级坐标系中的变换。

.. rst-class:: classref-item-separator

----

.. _class_Transform3D_method_rotated_local:

.. rst-class:: classref-method

:ref:`Transform3D<class_Transform3D>` **rotated_local** **(** :ref:`Vector3<class_Vector3>` axis, :ref:`float<class_float>` angle **)** |const|

返回该变换的副本，该副本围绕给定的 ``axis`` 轴进行了夹角为 ``angle`` 的旋转操作（单位为弧度）。

\ ``axis`` 必须为归一化的向量。

这个方法的结果和让 ``X`` 变换与相应的旋转变换 ``R`` 从右侧相乘一致，即 ``R * X``\ ，但进行了优化。

可以视作在局部坐标系中的变换。

.. rst-class:: classref-item-separator

----

.. _class_Transform3D_method_scaled:

.. rst-class:: classref-method

:ref:`Transform3D<class_Transform3D>` **scaled** **(** :ref:`Vector3<class_Vector3>` scale **)** |const|

返回该变换的副本，该副本进行了系数为 ``scale`` 的缩放操作。

这个方法的结果和让 ``X`` 变换与相应的缩放变换 ``S`` 从左侧相乘一致，即 ``S * X``\ ，但进行了优化。

可以视作在全局/父级坐标系中的变换。

.. rst-class:: classref-item-separator

----

.. _class_Transform3D_method_scaled_local:

.. rst-class:: classref-method

:ref:`Transform3D<class_Transform3D>` **scaled_local** **(** :ref:`Vector3<class_Vector3>` scale **)** |const|

返回该变换的副本，该副本进行了系数为 ``scale`` 的缩放操作。

这个方法的结果和让 ``X`` 变换与相应的缩放变换 ``S`` 从右侧相乘一致，即 ``X * S``\ ，但进行了优化。

可以视作在局部坐标系中的变换。

.. rst-class:: classref-item-separator

----

.. _class_Transform3D_method_translated:

.. rst-class:: classref-method

:ref:`Transform3D<class_Transform3D>` **translated** **(** :ref:`Vector3<class_Vector3>` offset **)** |const|

返回该变换的副本，该副本进行了偏移量为 ``offset`` 的平移操作。

这个方法的结果和让 ``X`` 变换与相应的平移变换 ``T`` 从左侧相乘一致，即 ``T * X``\ ，但进行了优化。

可以视作在全局/父级坐标系中的变换。

.. rst-class:: classref-item-separator

----

.. _class_Transform3D_method_translated_local:

.. rst-class:: classref-method

:ref:`Transform3D<class_Transform3D>` **translated_local** **(** :ref:`Vector3<class_Vector3>` offset **)** |const|

返回该变换的副本，该副本进行了偏移量为 ``offset`` 的平移操作。

这个方法的结果和让 ``X`` 变换与相应的平移变换 ``T`` 从右侧相乘一致，即 ``X * T``\ ，但进行了优化。

可以视作在局部坐标系中的变换。

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

操作符说明
----------

.. _class_Transform3D_operator_neq_Transform3D:

.. rst-class:: classref-operator

:ref:`bool<class_bool>` **operator !=** **(** :ref:`Transform3D<class_Transform3D>` right **)**

如果变换不相等，则返回 ``true``\ 。

\ **注意：**\ 由于浮点数精度误差，请考虑改用 :ref:`is_equal_approx<class_Transform3D_method_is_equal_approx>`\ ，会更可靠。

.. rst-class:: classref-item-separator

----

.. _class_Transform3D_operator_mul_AABB:

.. rst-class:: classref-operator

:ref:`AABB<class_AABB>` **operator *** **(** :ref:`AABB<class_AABB>` right **)**

使用给定的 **Transform3D** 矩阵对 :ref:`AABB<class_AABB>` 进行变换（相乘）。

.. rst-class:: classref-item-separator

----

.. _class_Transform3D_operator_mul_PackedVector3Array:

.. rst-class:: classref-operator

:ref:`PackedVector3Array<class_PackedVector3Array>` **operator *** **(** :ref:`PackedVector3Array<class_PackedVector3Array>` right **)**

使用给定的 **Transform3D** 矩阵对 :ref:`Vector3<class_Vector3>` 数组中的每个元素进行变换（相乘）。

.. rst-class:: classref-item-separator

----

.. _class_Transform3D_operator_mul_Plane:

.. rst-class:: classref-operator

:ref:`Plane<class_Plane>` **operator *** **(** :ref:`Plane<class_Plane>` right **)**

使用给定的 **Transform3D** 矩阵对 :ref:`Plane<class_Plane>` 进行变换（相乘）。

.. rst-class:: classref-item-separator

----

.. _class_Transform3D_operator_mul_Transform3D:

.. rst-class:: classref-operator

:ref:`Transform3D<class_Transform3D>` **operator *** **(** :ref:`Transform3D<class_Transform3D>` right **)**

通过将这两个变换矩阵相乘来组合它们。这具有通过第一个变换（父项）来变换第二个变换（子项）的效果。

.. rst-class:: classref-item-separator

----

.. _class_Transform3D_operator_mul_Vector3:

.. rst-class:: classref-operator

:ref:`Vector3<class_Vector3>` **operator *** **(** :ref:`Vector3<class_Vector3>` right **)**

使用给定的 **Transform3D** 矩阵对 :ref:`Vector3<class_Vector3>` 进行变换（相乘）。

.. rst-class:: classref-item-separator

----

.. _class_Transform3D_operator_mul_float:

.. rst-class:: classref-operator

:ref:`Transform3D<class_Transform3D>` **operator *** **(** :ref:`float<class_float>` right **)**

该运算符将 **Transform3D** 的所有分量相乘，包括 :ref:`origin<class_Transform3D_property_origin>` 向量，从而对其进行统一缩放。

.. rst-class:: classref-item-separator

----

.. _class_Transform3D_operator_mul_int:

.. rst-class:: classref-operator

:ref:`Transform3D<class_Transform3D>` **operator *** **(** :ref:`int<class_int>` right **)**

该运算符将 **Transform3D** 的所有分量相乘，包括 :ref:`origin<class_Transform3D_property_origin>` 向量，从而对其进行统一缩放。

.. rst-class:: classref-item-separator

----

.. _class_Transform3D_operator_eq_Transform3D:

.. rst-class:: classref-operator

:ref:`bool<class_bool>` **operator ==** **(** :ref:`Transform3D<class_Transform3D>` right **)**

如果变换完全相等，则返回 ``true``\ 。

\ **注意：**\ 由于浮点数精度误差，请考虑改用 :ref:`is_equal_approx<class_Transform3D_method_is_equal_approx>`\ ，会更可靠。

.. |virtual| replace:: :abbr:`virtual (本方法通常需要用户覆盖才能生效。)`
.. |const| replace:: :abbr:`const (本方法没有副作用。不会修改该实例的任何成员变量。)`
.. |vararg| replace:: :abbr:`vararg (本方法除了在此处描述的参数外，还能够继续接受任意数量的参数。)`
.. |constructor| replace:: :abbr:`constructor (本方法用于构造某个类型。)`
.. |static| replace:: :abbr:`static (调用本方法无需实例，所以可以直接使用类名调用。)`
.. |operator| replace:: :abbr:`operator (本方法描述的是使用本类型作为左操作数的有效操作符。)`
.. |bitfield| replace:: :abbr:`BitField (这个值是由下列标志构成的位掩码整数。)`
