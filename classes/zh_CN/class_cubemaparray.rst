:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/4.2/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/4.2/doc/classes/CubemapArray.xml.

.. _class_CubemapArray:

CubemapArray
============

**继承：** :ref:`ImageTextureLayered<class_ImageTextureLayered>` **<** :ref:`TextureLayered<class_TextureLayered>` **<** :ref:`Texture<class_Texture>` **<** :ref:`Resource<class_Resource>` **<** :ref:`RefCounted<class_RefCounted>` **<** :ref:`Object<class_Object>`

:ref:`Cubemap<class_Cubemap>` 数组，存储在一起并使用单个引用。

.. rst-class:: classref-introduction-group

描述
----

**CubemapArray** 由一组 :ref:`Cubemap<class_Cubemap>` 组成。它们像 :ref:`Cubemap<class_Cubemap>` 一样是由多个纹理组成的，其纹理的数量必须能被 6 整除（立方体的每个面都有一个）。\ **CubemapArray** 的主要好处是可以使用单个纹理引用在着色器代码中访问它们。换句话说，可以使用单个 **CubemapArray** 将多个 :ref:`Cubemap<class_Cubemap>` 传入着色器。

此外，\ :ref:`Cubemap<class_Cubemap>` 被分配在 GPU 上相邻的缓存区块中。这使得 **CubemapArray** 成为存储多个 :ref:`Cubemap<class_Cubemap>` 的最有效方式。

如果将 :ref:`ProjectSettings.rendering/reflections/sky_reflections/texture_array_reflections<class_ProjectSettings_property_rendering/reflections/sky_reflections/texture_array_reflections>` 设置为 ``true``\ ，Godot 在内部会将 **CubemapArray** 用于多种效果，包括 :ref:`Sky<class_Sky>`\ 。

要想自己创建这样的纹理文件，请使用文件系统停靠面板的导入预设重新导入你的图像文件。

\ **注意：**\ **CubemapArray** 在 OpenGL 3 渲染后端中不受支持。

.. rst-class:: classref-reftable-group

方法
----

.. table::
   :widths: auto

   +---------------------------------+---------------------------------------------------------------------------------------------+
   | :ref:`Resource<class_Resource>` | :ref:`create_placeholder<class_CubemapArray_method_create_placeholder>` **(** **)** |const| |
   +---------------------------------+---------------------------------------------------------------------------------------------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

方法说明
--------

.. _class_CubemapArray_method_create_placeholder:

.. rst-class:: classref-method

:ref:`Resource<class_Resource>` **create_placeholder** **(** **)** |const|

创建该资源的占位符版本（\ :ref:`PlaceholderCubemapArray<class_PlaceholderCubemapArray>`\ ）。

.. |virtual| replace:: :abbr:`virtual (本方法通常需要用户覆盖才能生效。)`
.. |const| replace:: :abbr:`const (本方法没有副作用。不会修改该实例的任何成员变量。)`
.. |vararg| replace:: :abbr:`vararg (本方法除了在此处描述的参数外，还能够继续接受任意数量的参数。)`
.. |constructor| replace:: :abbr:`constructor (本方法用于构造某个类型。)`
.. |static| replace:: :abbr:`static (调用本方法无需实例，所以可以直接使用类名调用。)`
.. |operator| replace:: :abbr:`operator (本方法描述的是使用本类型作为左操作数的有效操作符。)`
.. |bitfield| replace:: :abbr:`BitField (这个值是由下列标志构成的位掩码整数。)`
