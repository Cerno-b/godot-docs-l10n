:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/4.2/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/4.2/doc/classes/InputEventGesture.xml.

.. _class_InputEventGesture:

InputEventGesture
=================

**继承：** :ref:`InputEventWithModifiers<class_InputEventWithModifiers>` **<** :ref:`InputEventFromWindow<class_InputEventFromWindow>` **<** :ref:`InputEvent<class_InputEvent>` **<** :ref:`Resource<class_Resource>` **<** :ref:`RefCounted<class_RefCounted>` **<** :ref:`Object<class_Object>`

**派生：** :ref:`InputEventMagnifyGesture<class_InputEventMagnifyGesture>`, :ref:`InputEventPanGesture<class_InputEventPanGesture>`

触摸手势的抽象基类。

.. rst-class:: classref-introduction-group

描述
----

用户在触摸屏上执行支持的手势时会发送 InputEventGesture。无法用鼠标模拟手势，因为手势一般都要求多点触控。

.. rst-class:: classref-introduction-group

教程
----

- :doc:`使用 InputEvent <../tutorials/inputs/inputevent>`

.. rst-class:: classref-reftable-group

属性
----

.. table::
   :widths: auto

   +-------------------------------+------------------------------------------------------------+-------------------+
   | :ref:`Vector2<class_Vector2>` | :ref:`position<class_InputEventGesture_property_position>` | ``Vector2(0, 0)`` |
   +-------------------------------+------------------------------------------------------------+-------------------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

属性说明
--------

.. _class_InputEventGesture_property_position:

.. rst-class:: classref-property

:ref:`Vector2<class_Vector2>` **position** = ``Vector2(0, 0)``

.. rst-class:: classref-property-setget

- void **set_position** **(** :ref:`Vector2<class_Vector2>` value **)**
- :ref:`Vector2<class_Vector2>` **get_position** **(** **)**

相对于\ :ref:`Viewport<class_Viewport>`\ 的本地手势位置。如果在\ :ref:`Control._gui_input<class_Control_private_method__gui_input>`\ 中使用，位置是相对于当前接收该手势的控件\ :ref:`Control<class_Control>`\ 而言的。

.. |virtual| replace:: :abbr:`virtual (本方法通常需要用户覆盖才能生效。)`
.. |const| replace:: :abbr:`const (本方法没有副作用。不会修改该实例的任何成员变量。)`
.. |vararg| replace:: :abbr:`vararg (本方法除了在此处描述的参数外，还能够继续接受任意数量的参数。)`
.. |constructor| replace:: :abbr:`constructor (本方法用于构造某个类型。)`
.. |static| replace:: :abbr:`static (调用本方法无需实例，所以可以直接使用类名调用。)`
.. |operator| replace:: :abbr:`operator (本方法描述的是使用本类型作为左操作数的有效操作符。)`
.. |bitfield| replace:: :abbr:`BitField (这个值是由下列标志构成的位掩码整数。)`
