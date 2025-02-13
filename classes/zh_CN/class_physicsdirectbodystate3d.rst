:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/4.2/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/4.2/doc/classes/PhysicsDirectBodyState3D.xml.

.. _class_PhysicsDirectBodyState3D:

PhysicsDirectBodyState3D
========================

**继承：** :ref:`Object<class_Object>`

**派生：** :ref:`PhysicsDirectBodyState3DExtension<class_PhysicsDirectBodyState3DExtension>`

提供对 :ref:`PhysicsServer3D<class_PhysicsServer3D>` 中物理体的直接访问。

.. rst-class:: classref-introduction-group

描述
----

提供对 :ref:`PhysicsServer3D<class_PhysicsServer3D>` 中物理体的直接访问，从而安全地更改物理属性。该对象会在 :ref:`RigidBody3D<class_RigidBody3D>` 的直接状态回调中传递，目的是为了改变物体的直接状态。见 :ref:`RigidBody3D._integrate_forces<class_RigidBody3D_private_method__integrate_forces>`\ 。

.. rst-class:: classref-introduction-group

教程
----

- :doc:`物理介绍 <../tutorials/physics/physics_introduction>`

- :doc:`发射射线 <../tutorials/physics/ray-casting>`

.. rst-class:: classref-reftable-group

属性
----

.. table::
   :widths: auto

   +---------------------------------------+-----------------------------------------------------------------------------------------------+
   | :ref:`Vector3<class_Vector3>`         | :ref:`angular_velocity<class_PhysicsDirectBodyState3D_property_angular_velocity>`             |
   +---------------------------------------+-----------------------------------------------------------------------------------------------+
   | :ref:`Vector3<class_Vector3>`         | :ref:`center_of_mass<class_PhysicsDirectBodyState3D_property_center_of_mass>`                 |
   +---------------------------------------+-----------------------------------------------------------------------------------------------+
   | :ref:`Vector3<class_Vector3>`         | :ref:`center_of_mass_local<class_PhysicsDirectBodyState3D_property_center_of_mass_local>`     |
   +---------------------------------------+-----------------------------------------------------------------------------------------------+
   | :ref:`Vector3<class_Vector3>`         | :ref:`inverse_inertia<class_PhysicsDirectBodyState3D_property_inverse_inertia>`               |
   +---------------------------------------+-----------------------------------------------------------------------------------------------+
   | :ref:`Basis<class_Basis>`             | :ref:`inverse_inertia_tensor<class_PhysicsDirectBodyState3D_property_inverse_inertia_tensor>` |
   +---------------------------------------+-----------------------------------------------------------------------------------------------+
   | :ref:`float<class_float>`             | :ref:`inverse_mass<class_PhysicsDirectBodyState3D_property_inverse_mass>`                     |
   +---------------------------------------+-----------------------------------------------------------------------------------------------+
   | :ref:`Vector3<class_Vector3>`         | :ref:`linear_velocity<class_PhysicsDirectBodyState3D_property_linear_velocity>`               |
   +---------------------------------------+-----------------------------------------------------------------------------------------------+
   | :ref:`Basis<class_Basis>`             | :ref:`principal_inertia_axes<class_PhysicsDirectBodyState3D_property_principal_inertia_axes>` |
   +---------------------------------------+-----------------------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>`               | :ref:`sleeping<class_PhysicsDirectBodyState3D_property_sleeping>`                             |
   +---------------------------------------+-----------------------------------------------------------------------------------------------+
   | :ref:`float<class_float>`             | :ref:`step<class_PhysicsDirectBodyState3D_property_step>`                                     |
   +---------------------------------------+-----------------------------------------------------------------------------------------------+
   | :ref:`float<class_float>`             | :ref:`total_angular_damp<class_PhysicsDirectBodyState3D_property_total_angular_damp>`         |
   +---------------------------------------+-----------------------------------------------------------------------------------------------+
   | :ref:`Vector3<class_Vector3>`         | :ref:`total_gravity<class_PhysicsDirectBodyState3D_property_total_gravity>`                   |
   +---------------------------------------+-----------------------------------------------------------------------------------------------+
   | :ref:`float<class_float>`             | :ref:`total_linear_damp<class_PhysicsDirectBodyState3D_property_total_linear_damp>`           |
   +---------------------------------------+-----------------------------------------------------------------------------------------------+
   | :ref:`Transform3D<class_Transform3D>` | :ref:`transform<class_PhysicsDirectBodyState3D_property_transform>`                           |
   +---------------------------------------+-----------------------------------------------------------------------------------------------+

.. rst-class:: classref-reftable-group

方法
----

.. table::
   :widths: auto

   +-------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                                                              | :ref:`add_constant_central_force<class_PhysicsDirectBodyState3D_method_add_constant_central_force>` **(** :ref:`Vector3<class_Vector3>` force=Vector3(0, 0, 0) **)**                         |
   +-------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                                                              | :ref:`add_constant_force<class_PhysicsDirectBodyState3D_method_add_constant_force>` **(** :ref:`Vector3<class_Vector3>` force, :ref:`Vector3<class_Vector3>` position=Vector3(0, 0, 0) **)** |
   +-------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                                                              | :ref:`add_constant_torque<class_PhysicsDirectBodyState3D_method_add_constant_torque>` **(** :ref:`Vector3<class_Vector3>` torque **)**                                                       |
   +-------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                                                              | :ref:`apply_central_force<class_PhysicsDirectBodyState3D_method_apply_central_force>` **(** :ref:`Vector3<class_Vector3>` force=Vector3(0, 0, 0) **)**                                       |
   +-------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                                                              | :ref:`apply_central_impulse<class_PhysicsDirectBodyState3D_method_apply_central_impulse>` **(** :ref:`Vector3<class_Vector3>` impulse=Vector3(0, 0, 0) **)**                                 |
   +-------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                                                              | :ref:`apply_force<class_PhysicsDirectBodyState3D_method_apply_force>` **(** :ref:`Vector3<class_Vector3>` force, :ref:`Vector3<class_Vector3>` position=Vector3(0, 0, 0) **)**               |
   +-------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                                                              | :ref:`apply_impulse<class_PhysicsDirectBodyState3D_method_apply_impulse>` **(** :ref:`Vector3<class_Vector3>` impulse, :ref:`Vector3<class_Vector3>` position=Vector3(0, 0, 0) **)**         |
   +-------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                                                              | :ref:`apply_torque<class_PhysicsDirectBodyState3D_method_apply_torque>` **(** :ref:`Vector3<class_Vector3>` torque **)**                                                                     |
   +-------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                                                              | :ref:`apply_torque_impulse<class_PhysicsDirectBodyState3D_method_apply_torque_impulse>` **(** :ref:`Vector3<class_Vector3>` impulse **)**                                                    |
   +-------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Vector3<class_Vector3>`                                     | :ref:`get_constant_force<class_PhysicsDirectBodyState3D_method_get_constant_force>` **(** **)** |const|                                                                                      |
   +-------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Vector3<class_Vector3>`                                     | :ref:`get_constant_torque<class_PhysicsDirectBodyState3D_method_get_constant_torque>` **(** **)** |const|                                                                                    |
   +-------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`RID<class_RID>`                                             | :ref:`get_contact_collider<class_PhysicsDirectBodyState3D_method_get_contact_collider>` **(** :ref:`int<class_int>` contact_idx **)** |const|                                                |
   +-------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`int<class_int>`                                             | :ref:`get_contact_collider_id<class_PhysicsDirectBodyState3D_method_get_contact_collider_id>` **(** :ref:`int<class_int>` contact_idx **)** |const|                                          |
   +-------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Object<class_Object>`                                       | :ref:`get_contact_collider_object<class_PhysicsDirectBodyState3D_method_get_contact_collider_object>` **(** :ref:`int<class_int>` contact_idx **)** |const|                                  |
   +-------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Vector3<class_Vector3>`                                     | :ref:`get_contact_collider_position<class_PhysicsDirectBodyState3D_method_get_contact_collider_position>` **(** :ref:`int<class_int>` contact_idx **)** |const|                              |
   +-------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`int<class_int>`                                             | :ref:`get_contact_collider_shape<class_PhysicsDirectBodyState3D_method_get_contact_collider_shape>` **(** :ref:`int<class_int>` contact_idx **)** |const|                                    |
   +-------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Vector3<class_Vector3>`                                     | :ref:`get_contact_collider_velocity_at_position<class_PhysicsDirectBodyState3D_method_get_contact_collider_velocity_at_position>` **(** :ref:`int<class_int>` contact_idx **)** |const|      |
   +-------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`int<class_int>`                                             | :ref:`get_contact_count<class_PhysicsDirectBodyState3D_method_get_contact_count>` **(** **)** |const|                                                                                        |
   +-------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Vector3<class_Vector3>`                                     | :ref:`get_contact_impulse<class_PhysicsDirectBodyState3D_method_get_contact_impulse>` **(** :ref:`int<class_int>` contact_idx **)** |const|                                                  |
   +-------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Vector3<class_Vector3>`                                     | :ref:`get_contact_local_normal<class_PhysicsDirectBodyState3D_method_get_contact_local_normal>` **(** :ref:`int<class_int>` contact_idx **)** |const|                                        |
   +-------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Vector3<class_Vector3>`                                     | :ref:`get_contact_local_position<class_PhysicsDirectBodyState3D_method_get_contact_local_position>` **(** :ref:`int<class_int>` contact_idx **)** |const|                                    |
   +-------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`int<class_int>`                                             | :ref:`get_contact_local_shape<class_PhysicsDirectBodyState3D_method_get_contact_local_shape>` **(** :ref:`int<class_int>` contact_idx **)** |const|                                          |
   +-------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Vector3<class_Vector3>`                                     | :ref:`get_contact_local_velocity_at_position<class_PhysicsDirectBodyState3D_method_get_contact_local_velocity_at_position>` **(** :ref:`int<class_int>` contact_idx **)** |const|            |
   +-------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`PhysicsDirectSpaceState3D<class_PhysicsDirectSpaceState3D>` | :ref:`get_space_state<class_PhysicsDirectBodyState3D_method_get_space_state>` **(** **)**                                                                                                    |
   +-------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Vector3<class_Vector3>`                                     | :ref:`get_velocity_at_local_position<class_PhysicsDirectBodyState3D_method_get_velocity_at_local_position>` **(** :ref:`Vector3<class_Vector3>` local_position **)** |const|                 |
   +-------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                                                              | :ref:`integrate_forces<class_PhysicsDirectBodyState3D_method_integrate_forces>` **(** **)**                                                                                                  |
   +-------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                                                              | :ref:`set_constant_force<class_PhysicsDirectBodyState3D_method_set_constant_force>` **(** :ref:`Vector3<class_Vector3>` force **)**                                                          |
   +-------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                                                              | :ref:`set_constant_torque<class_PhysicsDirectBodyState3D_method_set_constant_torque>` **(** :ref:`Vector3<class_Vector3>` torque **)**                                                       |
   +-------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

属性说明
--------

.. _class_PhysicsDirectBodyState3D_property_angular_velocity:

.. rst-class:: classref-property

:ref:`Vector3<class_Vector3>` **angular_velocity**

.. rst-class:: classref-property-setget

- void **set_angular_velocity** **(** :ref:`Vector3<class_Vector3>` value **)**
- :ref:`Vector3<class_Vector3>` **get_angular_velocity** **(** **)**

物体的旋转速度，单位为\ *弧度*\ 每秒。

.. rst-class:: classref-item-separator

----

.. _class_PhysicsDirectBodyState3D_property_center_of_mass:

.. rst-class:: classref-property

:ref:`Vector3<class_Vector3>` **center_of_mass**

.. rst-class:: classref-property-setget

- :ref:`Vector3<class_Vector3>` **get_center_of_mass** **(** **)**

该物体质心的位置，相对于该物体的中心，使用全局坐标系。

.. rst-class:: classref-item-separator

----

.. _class_PhysicsDirectBodyState3D_property_center_of_mass_local:

.. rst-class:: classref-property

:ref:`Vector3<class_Vector3>` **center_of_mass_local**

.. rst-class:: classref-property-setget

- :ref:`Vector3<class_Vector3>` **get_center_of_mass_local** **(** **)**

该物体质心的位置，使用该物体的局部坐标系。

.. rst-class:: classref-item-separator

----

.. _class_PhysicsDirectBodyState3D_property_inverse_inertia:

.. rst-class:: classref-property

:ref:`Vector3<class_Vector3>` **inverse_inertia**

.. rst-class:: classref-property-setget

- :ref:`Vector3<class_Vector3>` **get_inverse_inertia** **(** **)**

物体惯性的倒数。

.. rst-class:: classref-item-separator

----

.. _class_PhysicsDirectBodyState3D_property_inverse_inertia_tensor:

.. rst-class:: classref-property

:ref:`Basis<class_Basis>` **inverse_inertia_tensor**

.. rst-class:: classref-property-setget

- :ref:`Basis<class_Basis>` **get_inverse_inertia_tensor** **(** **)**

该物体惯性张量的倒数。

.. rst-class:: classref-item-separator

----

.. _class_PhysicsDirectBodyState3D_property_inverse_mass:

.. rst-class:: classref-property

:ref:`float<class_float>` **inverse_mass**

.. rst-class:: classref-property-setget

- :ref:`float<class_float>` **get_inverse_mass** **(** **)**

物体质量的倒数。

.. rst-class:: classref-item-separator

----

.. _class_PhysicsDirectBodyState3D_property_linear_velocity:

.. rst-class:: classref-property

:ref:`Vector3<class_Vector3>` **linear_velocity**

.. rst-class:: classref-property-setget

- void **set_linear_velocity** **(** :ref:`Vector3<class_Vector3>` value **)**
- :ref:`Vector3<class_Vector3>` **get_linear_velocity** **(** **)**

物体的线速度，单位为单位每秒。

.. rst-class:: classref-item-separator

----

.. _class_PhysicsDirectBodyState3D_property_principal_inertia_axes:

.. rst-class:: classref-property

:ref:`Basis<class_Basis>` **principal_inertia_axes**

.. rst-class:: classref-property-setget

- :ref:`Basis<class_Basis>` **get_principal_inertia_axes** **(** **)**

.. container:: contribute

	目前没有这个属性的描述。请帮我们\ :ref:`贡献一个 <doc_updating_the_class_reference>`\ ！

.. rst-class:: classref-item-separator

----

.. _class_PhysicsDirectBodyState3D_property_sleeping:

.. rst-class:: classref-property

:ref:`bool<class_bool>` **sleeping**

.. rst-class:: classref-property-setget

- void **set_sleep_state** **(** :ref:`bool<class_bool>` value **)**
- :ref:`bool<class_bool>` **is_sleeping** **(** **)**

如果为 ``true``\ ，则该物体当前处于睡眠状态（不活动）。

.. rst-class:: classref-item-separator

----

.. _class_PhysicsDirectBodyState3D_property_step:

.. rst-class:: classref-property

:ref:`float<class_float>` **step**

.. rst-class:: classref-property-setget

- :ref:`float<class_float>` **get_step** **(** **)**

用于模拟的时间步长（delta）。

.. rst-class:: classref-item-separator

----

.. _class_PhysicsDirectBodyState3D_property_total_angular_damp:

.. rst-class:: classref-property

:ref:`float<class_float>` **total_angular_damp**

.. rst-class:: classref-property-setget

- :ref:`float<class_float>` **get_total_angular_damp** **(** **)**

物体停止转动的速度，如果没有任何其他力使它运动。

.. rst-class:: classref-item-separator

----

.. _class_PhysicsDirectBodyState3D_property_total_gravity:

.. rst-class:: classref-property

:ref:`Vector3<class_Vector3>` **total_gravity**

.. rst-class:: classref-property-setget

- :ref:`Vector3<class_Vector3>` **get_total_gravity** **(** **)**

这个物体上的总重力向量。

.. rst-class:: classref-item-separator

----

.. _class_PhysicsDirectBodyState3D_property_total_linear_damp:

.. rst-class:: classref-property

:ref:`float<class_float>` **total_linear_damp**

.. rst-class:: classref-property-setget

- :ref:`float<class_float>` **get_total_linear_damp** **(** **)**

物体停止运动的速率，如果没有任何其他力使它运动。

.. rst-class:: classref-item-separator

----

.. _class_PhysicsDirectBodyState3D_property_transform:

.. rst-class:: classref-property

:ref:`Transform3D<class_Transform3D>` **transform**

.. rst-class:: classref-property-setget

- void **set_transform** **(** :ref:`Transform3D<class_Transform3D>` value **)**
- :ref:`Transform3D<class_Transform3D>` **get_transform** **(** **)**

物体的变换矩阵。

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

方法说明
--------

.. _class_PhysicsDirectBodyState3D_method_add_constant_central_force:

.. rst-class:: classref-method

void **add_constant_central_force** **(** :ref:`Vector3<class_Vector3>` force=Vector3(0, 0, 0) **)**

在不影响旋转的情况下，添加一个恒定的定向力，该力会随着时间的推移而持续施加，直到使用 ``constant_force = Vector3(0, 0, 0)`` 清除。

这相当于在物体的质心处，使用 :ref:`add_constant_force<class_PhysicsDirectBodyState3D_method_add_constant_force>`\ 。

.. rst-class:: classref-item-separator

----

.. _class_PhysicsDirectBodyState3D_method_add_constant_force:

.. rst-class:: classref-method

void **add_constant_force** **(** :ref:`Vector3<class_Vector3>` force, :ref:`Vector3<class_Vector3>` position=Vector3(0, 0, 0) **)**

向实体添加一个恒定的定位力，持续施加，直到用 ``constant_force = Vector3(0, 0, 0)`` 清除。

\ ``position`` 是在全局坐标中距实体原点的偏移量。

.. rst-class:: classref-item-separator

----

.. _class_PhysicsDirectBodyState3D_method_add_constant_torque:

.. rst-class:: classref-method

void **add_constant_torque** **(** :ref:`Vector3<class_Vector3>` torque **)**

在不影响位置的情况下，添加一个恒定的旋转力，该力会随着时间的推移而持续施加，直到使用 ``constant_torque = Vector3(0, 0, 0)`` 清除。

.. rst-class:: classref-item-separator

----

.. _class_PhysicsDirectBodyState3D_method_apply_central_force:

.. rst-class:: classref-method

void **apply_central_force** **(** :ref:`Vector3<class_Vector3>` force=Vector3(0, 0, 0) **)**

施加一个不影响旋转的定向力。该力是时间相关的，意味着每次物理更新都会施加。

这相当于在物体的质心处，使用 :ref:`apply_force<class_PhysicsDirectBodyState3D_method_apply_force>`\ 。

.. rst-class:: classref-item-separator

----

.. _class_PhysicsDirectBodyState3D_method_apply_central_impulse:

.. rst-class:: classref-method

void **apply_central_impulse** **(** :ref:`Vector3<class_Vector3>` impulse=Vector3(0, 0, 0) **)**

施加一个不影响的旋转定向冲量。

冲量与时间无关！每帧应用一个冲量，会产生一个依赖于帧速率的力。出于这个原因，它应该只在模拟一次性影响时使用（否则使用 “_force”函数）。

这相当于在物体的质心处，使用 :ref:`apply_impulse<class_PhysicsDirectBodyState3D_method_apply_impulse>`\ 。

.. rst-class:: classref-item-separator

----

.. _class_PhysicsDirectBodyState3D_method_apply_force:

.. rst-class:: classref-method

void **apply_force** **(** :ref:`Vector3<class_Vector3>` force, :ref:`Vector3<class_Vector3>` position=Vector3(0, 0, 0) **)**

对实体施加一个定位力。力是时间相关的，意味着每次物理更新都会被施加。

\ ``position`` 是在全局坐标中距实体原点的偏移量。

.. rst-class:: classref-item-separator

----

.. _class_PhysicsDirectBodyState3D_method_apply_impulse:

.. rst-class:: classref-method

void **apply_impulse** **(** :ref:`Vector3<class_Vector3>` impulse, :ref:`Vector3<class_Vector3>` position=Vector3(0, 0, 0) **)**

向实体施加一个定位冲量。

冲量是时间无关的！每帧施加一个冲量将产生一个依赖于帧速率的力。出于这个原因，它应该只在模拟一次性影响时使用（否则使用“_force”函数）。

\ ``position`` 是在全局坐标中距实体原点的偏移量。

.. rst-class:: classref-item-separator

----

.. _class_PhysicsDirectBodyState3D_method_apply_torque:

.. rst-class:: classref-method

void **apply_torque** **(** :ref:`Vector3<class_Vector3>` torque **)**

在不影响位置的情况下，施加一个旋转力。该力是与时间相关的，这意味着每次物理更新时都会被施加。

\ **注意：**\ :ref:`inverse_inertia<class_PhysicsDirectBodyState3D_property_inverse_inertia>` 是该函数生效所必需的。要拥有 :ref:`inverse_inertia<class_PhysicsDirectBodyState3D_property_inverse_inertia>`\ ，一个活动的 :ref:`CollisionShape3D<class_CollisionShape3D>` 必须是该节点的子节点，或者可以手动设置 :ref:`inverse_inertia<class_PhysicsDirectBodyState3D_property_inverse_inertia>`\ 。

.. rst-class:: classref-item-separator

----

.. _class_PhysicsDirectBodyState3D_method_apply_torque_impulse:

.. rst-class:: classref-method

void **apply_torque_impulse** **(** :ref:`Vector3<class_Vector3>` impulse **)**

在不影响位置的情况下，向实体施加一个旋转冲量。

冲量是时间无关的！每帧施加一个冲量将产生一个依赖于帧速率的力。出于这个原因，它应该只在模拟一次性影响时使用（否则使用“_force”函数）。

\ **注意：**\ :ref:`inverse_inertia<class_PhysicsDirectBodyState3D_property_inverse_inertia>` 是生效所必需的。要拥有 :ref:`inverse_inertia<class_PhysicsDirectBodyState3D_property_inverse_inertia>`\ ，活动的 :ref:`CollisionShape3D<class_CollisionShape3D>` 必须是该节点的子节点，或者可以手动设置 :ref:`inverse_inertia<class_PhysicsDirectBodyState3D_property_inverse_inertia>`\ 。

.. rst-class:: classref-item-separator

----

.. _class_PhysicsDirectBodyState3D_method_get_constant_force:

.. rst-class:: classref-method

:ref:`Vector3<class_Vector3>` **get_constant_force** **(** **)** |const|

返回在每次物理更新期间，施加在该物体上的总恒定位置力。

见 :ref:`add_constant_force<class_PhysicsDirectBodyState3D_method_add_constant_force>` 和 :ref:`add_constant_central_force<class_PhysicsDirectBodyState3D_method_add_constant_central_force>`\ 。

.. rst-class:: classref-item-separator

----

.. _class_PhysicsDirectBodyState3D_method_get_constant_torque:

.. rst-class:: classref-method

:ref:`Vector3<class_Vector3>` **get_constant_torque** **(** **)** |const|

返回在每次物理更新期间，施加在该物体上的总恒定旋转力。

见 :ref:`add_constant_torque<class_PhysicsDirectBodyState3D_method_add_constant_torque>`\ 。

.. rst-class:: classref-item-separator

----

.. _class_PhysicsDirectBodyState3D_method_get_contact_collider:

.. rst-class:: classref-method

:ref:`RID<class_RID>` **get_contact_collider** **(** :ref:`int<class_int>` contact_idx **)** |const|

返回该碰撞体的 :ref:`RID<class_RID>`\ 。

.. rst-class:: classref-item-separator

----

.. _class_PhysicsDirectBodyState3D_method_get_contact_collider_id:

.. rst-class:: classref-method

:ref:`int<class_int>` **get_contact_collider_id** **(** :ref:`int<class_int>` contact_idx **)** |const|

返回该碰撞体的对象 id。

.. rst-class:: classref-item-separator

----

.. _class_PhysicsDirectBodyState3D_method_get_contact_collider_object:

.. rst-class:: classref-method

:ref:`Object<class_Object>` **get_contact_collider_object** **(** :ref:`int<class_int>` contact_idx **)** |const|

返回碰撞对象。

.. rst-class:: classref-item-separator

----

.. _class_PhysicsDirectBodyState3D_method_get_contact_collider_position:

.. rst-class:: classref-method

:ref:`Vector3<class_Vector3>` **get_contact_collider_position** **(** :ref:`int<class_int>` contact_idx **)** |const|

返回该碰撞体上接触点的位置，使用全局坐标系。

.. rst-class:: classref-item-separator

----

.. _class_PhysicsDirectBodyState3D_method_get_contact_collider_shape:

.. rst-class:: classref-method

:ref:`int<class_int>` **get_contact_collider_shape** **(** :ref:`int<class_int>` contact_idx **)** |const|

返回该碰撞体的形状索引。

.. rst-class:: classref-item-separator

----

.. _class_PhysicsDirectBodyState3D_method_get_contact_collider_velocity_at_position:

.. rst-class:: classref-method

:ref:`Vector3<class_Vector3>` **get_contact_collider_velocity_at_position** **(** :ref:`int<class_int>` contact_idx **)** |const|

返回该碰撞体接触点处的线速度向量。

.. rst-class:: classref-item-separator

----

.. _class_PhysicsDirectBodyState3D_method_get_contact_count:

.. rst-class:: classref-method

:ref:`int<class_int>` **get_contact_count** **(** **)** |const|

返回这个物体与其他物体的接触次数。

\ **注意：**\ 默认情况下，除非物体被设为监视接触，否则会返回 0。见 :ref:`RigidBody3D.contact_monitor<class_RigidBody3D_property_contact_monitor>`\ 。

.. rst-class:: classref-item-separator

----

.. _class_PhysicsDirectBodyState3D_method_get_contact_impulse:

.. rst-class:: classref-method

:ref:`Vector3<class_Vector3>` **get_contact_impulse** **(** :ref:`int<class_int>` contact_idx **)** |const|

由接触产生的冲量。

.. rst-class:: classref-item-separator

----

.. _class_PhysicsDirectBodyState3D_method_get_contact_local_normal:

.. rst-class:: classref-method

:ref:`Vector3<class_Vector3>` **get_contact_local_normal** **(** :ref:`int<class_int>` contact_idx **)** |const|

返回接触点处的局部法线。

.. rst-class:: classref-item-separator

----

.. _class_PhysicsDirectBodyState3D_method_get_contact_local_position:

.. rst-class:: classref-method

:ref:`Vector3<class_Vector3>` **get_contact_local_position** **(** :ref:`int<class_int>` contact_idx **)** |const|

返回该物体上接触点的位置，使用全局坐标系。

.. rst-class:: classref-item-separator

----

.. _class_PhysicsDirectBodyState3D_method_get_contact_local_shape:

.. rst-class:: classref-method

:ref:`int<class_int>` **get_contact_local_shape** **(** :ref:`int<class_int>` contact_idx **)** |const|

返回碰撞的局部坐标系下的形状索引。

.. rst-class:: classref-item-separator

----

.. _class_PhysicsDirectBodyState3D_method_get_contact_local_velocity_at_position:

.. rst-class:: classref-method

:ref:`Vector3<class_Vector3>` **get_contact_local_velocity_at_position** **(** :ref:`int<class_int>` contact_idx **)** |const|

返回该物体上接触点处的线速度向量。

.. rst-class:: classref-item-separator

----

.. _class_PhysicsDirectBodyState3D_method_get_space_state:

.. rst-class:: classref-method

:ref:`PhysicsDirectSpaceState3D<class_PhysicsDirectSpaceState3D>` **get_space_state** **(** **)**

返回空间的当前状态，这对查询很有用。

.. rst-class:: classref-item-separator

----

.. _class_PhysicsDirectBodyState3D_method_get_velocity_at_local_position:

.. rst-class:: classref-method

:ref:`Vector3<class_Vector3>` **get_velocity_at_local_position** **(** :ref:`Vector3<class_Vector3>` local_position **)** |const|

返回给定相对位置的物体速度，包括平移和旋转。

.. rst-class:: classref-item-separator

----

.. _class_PhysicsDirectBodyState3D_method_integrate_forces:

.. rst-class:: classref-method

void **integrate_forces** **(** **)**

调用内置的力集成代码。

.. rst-class:: classref-item-separator

----

.. _class_PhysicsDirectBodyState3D_method_set_constant_force:

.. rst-class:: classref-method

void **set_constant_force** **(** :ref:`Vector3<class_Vector3>` force **)**

设置在每次物理更新期间，施加在该物体上的总恒定位置力。

见 :ref:`add_constant_force<class_PhysicsDirectBodyState3D_method_add_constant_force>` 和 :ref:`add_constant_central_force<class_PhysicsDirectBodyState3D_method_add_constant_central_force>`\ 。

.. rst-class:: classref-item-separator

----

.. _class_PhysicsDirectBodyState3D_method_set_constant_torque:

.. rst-class:: classref-method

void **set_constant_torque** **(** :ref:`Vector3<class_Vector3>` torque **)**

设置在每次物理更新期间，施加在该物体上的总恒定旋转力。

见 :ref:`add_constant_torque<class_PhysicsDirectBodyState3D_method_add_constant_torque>`\ 。

.. |virtual| replace:: :abbr:`virtual (本方法通常需要用户覆盖才能生效。)`
.. |const| replace:: :abbr:`const (本方法没有副作用。不会修改该实例的任何成员变量。)`
.. |vararg| replace:: :abbr:`vararg (本方法除了在此处描述的参数外，还能够继续接受任意数量的参数。)`
.. |constructor| replace:: :abbr:`constructor (本方法用于构造某个类型。)`
.. |static| replace:: :abbr:`static (调用本方法无需实例，所以可以直接使用类名调用。)`
.. |operator| replace:: :abbr:`operator (本方法描述的是使用本类型作为左操作数的有效操作符。)`
.. |bitfield| replace:: :abbr:`BitField (这个值是由下列标志构成的位掩码整数。)`
