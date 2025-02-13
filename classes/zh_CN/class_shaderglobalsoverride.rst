:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/4.2/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/4.2/doc/classes/ShaderGlobalsOverride.xml.

.. _class_ShaderGlobalsOverride:

ShaderGlobalsOverride
=====================

**继承：** :ref:`Node<class_Node>` **<** :ref:`Object<class_Object>`

在场景中覆盖全局着色器参数取值的节点。

.. rst-class:: classref-introduction-group

描述
----

就像 :ref:`WorldEnvironment<class_WorldEnvironment>` 能够在加载指定场景时覆盖环境一样，\ **ShaderGlobalsOverride** 能够临时覆盖全局着色器参数。移除该节点后，就会恢复项目范围的全局着色器参数。详情见 :ref:`RenderingServer<class_RenderingServer>` 的 ``global_shader_parameter_*`` 方法。

\ **注意：**\ 一个场景只能用一个 **ShaderGlobalsOverride**\ 。如果场景树中存在多个 **ShaderGlobalsOverride**\ ，则只会考虑第一个节点（按照树顺序）。

\ **注意：**\ 所有 **ShaderGlobalsOverride** 节点在添加至场景树时都会加入 ``"shader_overrides_group"`` 分组。当前活动的 **ShaderGlobalsOverride** 还会加入 ``"shader_overrides_group_active"`` 分组。你可以据此来检查当前活动的 **ShaderGlobalsOverride** 节点是哪一个。

.. rst-class:: classref-introduction-group

教程
----

- :doc:`着色语言 <../tutorials/shaders/shader_reference/shading_language>`

.. |virtual| replace:: :abbr:`virtual (本方法通常需要用户覆盖才能生效。)`
.. |const| replace:: :abbr:`const (本方法没有副作用。不会修改该实例的任何成员变量。)`
.. |vararg| replace:: :abbr:`vararg (本方法除了在此处描述的参数外，还能够继续接受任意数量的参数。)`
.. |constructor| replace:: :abbr:`constructor (本方法用于构造某个类型。)`
.. |static| replace:: :abbr:`static (调用本方法无需实例，所以可以直接使用类名调用。)`
.. |operator| replace:: :abbr:`operator (本方法描述的是使用本类型作为左操作数的有效操作符。)`
.. |bitfield| replace:: :abbr:`BitField (这个值是由下列标志构成的位掩码整数。)`
