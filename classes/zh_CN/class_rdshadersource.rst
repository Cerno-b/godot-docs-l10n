:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/4.2/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/4.2/doc/classes/RDShaderSource.xml.

.. _class_RDShaderSource:

RDShaderSource
==============

**继承：** :ref:`RefCounted<class_RefCounted>` **<** :ref:`Object<class_Object>`

着色器源代码（由 :ref:`RenderingDevice<class_RenderingDevice>` 使用）。

.. rst-class:: classref-introduction-group

描述
----

文本形式的着色器源代码。

另见 :ref:`RDShaderFile<class_RDShaderFile>`\ 。\ **RDShaderSource** 应该仅用于 :ref:`RenderingDevice<class_RenderingDevice>` API。不应将其与 Godot 自己的 :ref:`Shader<class_Shader>` 资源，Godot 的各种节点会使用后者来进行高阶着色器编程。

.. rst-class:: classref-reftable-group

属性
----

.. table::
   :widths: auto

   +------------------------------------------------------------+---------------------------------------------------------------------------------------------------+--------+
   | :ref:`ShaderLanguage<enum_RenderingDevice_ShaderLanguage>` | :ref:`language<class_RDShaderSource_property_language>`                                           | ``0``  |
   +------------------------------------------------------------+---------------------------------------------------------------------------------------------------+--------+
   | :ref:`String<class_String>`                                | :ref:`source_compute<class_RDShaderSource_property_source_compute>`                               | ``""`` |
   +------------------------------------------------------------+---------------------------------------------------------------------------------------------------+--------+
   | :ref:`String<class_String>`                                | :ref:`source_fragment<class_RDShaderSource_property_source_fragment>`                             | ``""`` |
   +------------------------------------------------------------+---------------------------------------------------------------------------------------------------+--------+
   | :ref:`String<class_String>`                                | :ref:`source_tesselation_control<class_RDShaderSource_property_source_tesselation_control>`       | ``""`` |
   +------------------------------------------------------------+---------------------------------------------------------------------------------------------------+--------+
   | :ref:`String<class_String>`                                | :ref:`source_tesselation_evaluation<class_RDShaderSource_property_source_tesselation_evaluation>` | ``""`` |
   +------------------------------------------------------------+---------------------------------------------------------------------------------------------------+--------+
   | :ref:`String<class_String>`                                | :ref:`source_vertex<class_RDShaderSource_property_source_vertex>`                                 | ``""`` |
   +------------------------------------------------------------+---------------------------------------------------------------------------------------------------+--------+

.. rst-class:: classref-reftable-group

方法
----

.. table::
   :widths: auto

   +-----------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`String<class_String>` | :ref:`get_stage_source<class_RDShaderSource_method_get_stage_source>` **(** :ref:`ShaderStage<enum_RenderingDevice_ShaderStage>` stage **)** |const|                             |
   +-----------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                        | :ref:`set_stage_source<class_RDShaderSource_method_set_stage_source>` **(** :ref:`ShaderStage<enum_RenderingDevice_ShaderStage>` stage, :ref:`String<class_String>` source **)** |
   +-----------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

属性说明
--------

.. _class_RDShaderSource_property_language:

.. rst-class:: classref-property

:ref:`ShaderLanguage<enum_RenderingDevice_ShaderLanguage>` **language** = ``0``

.. rst-class:: classref-property-setget

- void **set_language** **(** :ref:`ShaderLanguage<enum_RenderingDevice_ShaderLanguage>` value **)**
- :ref:`ShaderLanguage<enum_RenderingDevice_ShaderLanguage>` **get_language** **(** **)**

着色器的编写语言。

.. rst-class:: classref-item-separator

----

.. _class_RDShaderSource_property_source_compute:

.. rst-class:: classref-property

:ref:`String<class_String>` **source_compute** = ``""``

.. rst-class:: classref-property-setget

- void **set_stage_source** **(** :ref:`ShaderStage<enum_RenderingDevice_ShaderStage>` stage, :ref:`String<class_String>` source **)**
- :ref:`String<class_String>` **get_stage_source** **(** :ref:`ShaderStage<enum_RenderingDevice_ShaderStage>` stage **)** |const|

着色器计算阶段的源代码。

.. rst-class:: classref-item-separator

----

.. _class_RDShaderSource_property_source_fragment:

.. rst-class:: classref-property

:ref:`String<class_String>` **source_fragment** = ``""``

.. rst-class:: classref-property-setget

- void **set_stage_source** **(** :ref:`ShaderStage<enum_RenderingDevice_ShaderStage>` stage, :ref:`String<class_String>` source **)**
- :ref:`String<class_String>` **get_stage_source** **(** :ref:`ShaderStage<enum_RenderingDevice_ShaderStage>` stage **)** |const|

着色器片段阶段的源代码。

.. rst-class:: classref-item-separator

----

.. _class_RDShaderSource_property_source_tesselation_control:

.. rst-class:: classref-property

:ref:`String<class_String>` **source_tesselation_control** = ``""``

.. rst-class:: classref-property-setget

- void **set_stage_source** **(** :ref:`ShaderStage<enum_RenderingDevice_ShaderStage>` stage, :ref:`String<class_String>` source **)**
- :ref:`String<class_String>` **get_stage_source** **(** :ref:`ShaderStage<enum_RenderingDevice_ShaderStage>` stage **)** |const|

着色器曲面细分控制阶段的源代码。

.. rst-class:: classref-item-separator

----

.. _class_RDShaderSource_property_source_tesselation_evaluation:

.. rst-class:: classref-property

:ref:`String<class_String>` **source_tesselation_evaluation** = ``""``

.. rst-class:: classref-property-setget

- void **set_stage_source** **(** :ref:`ShaderStage<enum_RenderingDevice_ShaderStage>` stage, :ref:`String<class_String>` source **)**
- :ref:`String<class_String>` **get_stage_source** **(** :ref:`ShaderStage<enum_RenderingDevice_ShaderStage>` stage **)** |const|

着色器曲面细分求值阶段的源代码。

.. rst-class:: classref-item-separator

----

.. _class_RDShaderSource_property_source_vertex:

.. rst-class:: classref-property

:ref:`String<class_String>` **source_vertex** = ``""``

.. rst-class:: classref-property-setget

- void **set_stage_source** **(** :ref:`ShaderStage<enum_RenderingDevice_ShaderStage>` stage, :ref:`String<class_String>` source **)**
- :ref:`String<class_String>` **get_stage_source** **(** :ref:`ShaderStage<enum_RenderingDevice_ShaderStage>` stage **)** |const|

着色器顶点阶段的源代码。

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

方法说明
--------

.. _class_RDShaderSource_method_get_stage_source:

.. rst-class:: classref-method

:ref:`String<class_String>` **get_stage_source** **(** :ref:`ShaderStage<enum_RenderingDevice_ShaderStage>` stage **)** |const|

返回指定着色器阶段 ``stage`` 的源代码。等价于获取 :ref:`source_compute<class_RDShaderSource_property_source_compute>`\ 、\ :ref:`source_fragment<class_RDShaderSource_property_source_fragment>`\ 、\ :ref:`source_tesselation_control<class_RDShaderSource_property_source_tesselation_control>`\ 、\ :ref:`source_tesselation_evaluation<class_RDShaderSource_property_source_tesselation_evaluation>` 或 :ref:`source_vertex<class_RDShaderSource_property_source_vertex>`\ 。

.. rst-class:: classref-item-separator

----

.. _class_RDShaderSource_method_set_stage_source:

.. rst-class:: classref-method

void **set_stage_source** **(** :ref:`ShaderStage<enum_RenderingDevice_ShaderStage>` stage, :ref:`String<class_String>` source **)**

设置指定着色器阶段 ``stage`` 的源代码 ``source``\ 。等价于设置 :ref:`source_compute<class_RDShaderSource_property_source_compute>`\ 、\ :ref:`source_fragment<class_RDShaderSource_property_source_fragment>`\ 、\ :ref:`source_tesselation_control<class_RDShaderSource_property_source_tesselation_control>`\ 、\ :ref:`source_tesselation_evaluation<class_RDShaderSource_property_source_tesselation_evaluation>` 或 :ref:`source_vertex<class_RDShaderSource_property_source_vertex>`\ 。

.. |virtual| replace:: :abbr:`virtual (本方法通常需要用户覆盖才能生效。)`
.. |const| replace:: :abbr:`const (本方法没有副作用。不会修改该实例的任何成员变量。)`
.. |vararg| replace:: :abbr:`vararg (本方法除了在此处描述的参数外，还能够继续接受任意数量的参数。)`
.. |constructor| replace:: :abbr:`constructor (本方法用于构造某个类型。)`
.. |static| replace:: :abbr:`static (调用本方法无需实例，所以可以直接使用类名调用。)`
.. |operator| replace:: :abbr:`operator (本方法描述的是使用本类型作为左操作数的有效操作符。)`
.. |bitfield| replace:: :abbr:`BitField (这个值是由下列标志构成的位掩码整数。)`
