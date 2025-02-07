:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/4.2/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/4.2/doc/classes/SpriteFrames.xml.

.. _class_SpriteFrames:

SpriteFrames
============

**继承：** :ref:`Resource<class_Resource>` **<** :ref:`RefCounted<class_RefCounted>` **<** :ref:`Object<class_Object>`

精灵帧库，用于 AnimatedSprite2D 和 AnimatedSprite3D。

.. rst-class:: classref-introduction-group

描述
----

:ref:`AnimatedSprite2D<class_AnimatedSprite2D>` 和 :ref:`AnimatedSprite3D<class_AnimatedSprite3D>` 节点的精灵帧库。包含帧和用于播放的动画信息。

.. rst-class:: classref-reftable-group

方法
----

.. table::
   :widths: auto

   +---------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                                              | :ref:`add_animation<class_SpriteFrames_method_add_animation>` **(** :ref:`StringName<class_StringName>` anim **)**                                                                                                                  |
   +---------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                                              | :ref:`add_frame<class_SpriteFrames_method_add_frame>` **(** :ref:`StringName<class_StringName>` anim, :ref:`Texture2D<class_Texture2D>` texture, :ref:`float<class_float>` duration=1.0, :ref:`int<class_int>` at_position=-1 **)** |
   +---------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                                              | :ref:`clear<class_SpriteFrames_method_clear>` **(** :ref:`StringName<class_StringName>` anim **)**                                                                                                                                  |
   +---------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                                              | :ref:`clear_all<class_SpriteFrames_method_clear_all>` **(** **)**                                                                                                                                                                   |
   +---------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>`                           | :ref:`get_animation_loop<class_SpriteFrames_method_get_animation_loop>` **(** :ref:`StringName<class_StringName>` anim **)** |const|                                                                                                |
   +---------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`PackedStringArray<class_PackedStringArray>` | :ref:`get_animation_names<class_SpriteFrames_method_get_animation_names>` **(** **)** |const|                                                                                                                                       |
   +---------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`float<class_float>`                         | :ref:`get_animation_speed<class_SpriteFrames_method_get_animation_speed>` **(** :ref:`StringName<class_StringName>` anim **)** |const|                                                                                              |
   +---------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`int<class_int>`                             | :ref:`get_frame_count<class_SpriteFrames_method_get_frame_count>` **(** :ref:`StringName<class_StringName>` anim **)** |const|                                                                                                      |
   +---------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`float<class_float>`                         | :ref:`get_frame_duration<class_SpriteFrames_method_get_frame_duration>` **(** :ref:`StringName<class_StringName>` anim, :ref:`int<class_int>` idx **)** |const|                                                                     |
   +---------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`Texture2D<class_Texture2D>`                 | :ref:`get_frame_texture<class_SpriteFrames_method_get_frame_texture>` **(** :ref:`StringName<class_StringName>` anim, :ref:`int<class_int>` idx **)** |const|                                                                       |
   +---------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`bool<class_bool>`                           | :ref:`has_animation<class_SpriteFrames_method_has_animation>` **(** :ref:`StringName<class_StringName>` anim **)** |const|                                                                                                          |
   +---------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                                              | :ref:`remove_animation<class_SpriteFrames_method_remove_animation>` **(** :ref:`StringName<class_StringName>` anim **)**                                                                                                            |
   +---------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                                              | :ref:`remove_frame<class_SpriteFrames_method_remove_frame>` **(** :ref:`StringName<class_StringName>` anim, :ref:`int<class_int>` idx **)**                                                                                         |
   +---------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                                              | :ref:`rename_animation<class_SpriteFrames_method_rename_animation>` **(** :ref:`StringName<class_StringName>` anim, :ref:`StringName<class_StringName>` newname **)**                                                               |
   +---------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                                              | :ref:`set_animation_loop<class_SpriteFrames_method_set_animation_loop>` **(** :ref:`StringName<class_StringName>` anim, :ref:`bool<class_bool>` loop **)**                                                                          |
   +---------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                                              | :ref:`set_animation_speed<class_SpriteFrames_method_set_animation_speed>` **(** :ref:`StringName<class_StringName>` anim, :ref:`float<class_float>` fps **)**                                                                       |
   +---------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | void                                              | :ref:`set_frame<class_SpriteFrames_method_set_frame>` **(** :ref:`StringName<class_StringName>` anim, :ref:`int<class_int>` idx, :ref:`Texture2D<class_Texture2D>` texture, :ref:`float<class_float>` duration=1.0 **)**            |
   +---------------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

方法说明
--------

.. _class_SpriteFrames_method_add_animation:

.. rst-class:: classref-method

void **add_animation** **(** :ref:`StringName<class_StringName>` anim **)**

向库中添加新动画 ``anim``\ 。

.. rst-class:: classref-item-separator

----

.. _class_SpriteFrames_method_add_frame:

.. rst-class:: classref-method

void **add_frame** **(** :ref:`StringName<class_StringName>` anim, :ref:`Texture2D<class_Texture2D>` texture, :ref:`float<class_float>` duration=1.0, :ref:`int<class_int>` at_position=-1 **)**

向 ``anim`` 动画中添加一帧。如果 ``at_position`` 为 ``-1``\ ，则该帧会添加至该动画的末尾。

.. rst-class:: classref-item-separator

----

.. _class_SpriteFrames_method_clear:

.. rst-class:: classref-method

void **clear** **(** :ref:`StringName<class_StringName>` anim **)**

删除 ``anim`` 动画中的所有帧。

.. rst-class:: classref-item-separator

----

.. _class_SpriteFrames_method_clear_all:

.. rst-class:: classref-method

void **clear_all** **(** **)**

移除所有动画。将创建名为 ``default`` 的空动画。

.. rst-class:: classref-item-separator

----

.. _class_SpriteFrames_method_get_animation_loop:

.. rst-class:: classref-method

:ref:`bool<class_bool>` **get_animation_loop** **(** :ref:`StringName<class_StringName>` anim **)** |const|

当指定的动画被配置为结束播放后循环时，返回 ``true``\ ，否则返回 ``false``\ 。

.. rst-class:: classref-item-separator

----

.. _class_SpriteFrames_method_get_animation_names:

.. rst-class:: classref-method

:ref:`PackedStringArray<class_PackedStringArray>` **get_animation_names** **(** **)** |const|

返回一个包含每个动画的名称的数组。值按字母顺序排列。

.. rst-class:: classref-item-separator

----

.. _class_SpriteFrames_method_get_animation_speed:

.. rst-class:: classref-method

:ref:`float<class_float>` **get_animation_speed** **(** :ref:`StringName<class_StringName>` anim **)** |const|

返回 ``anim`` 动画的速度，单位为帧每秒。

.. rst-class:: classref-item-separator

----

.. _class_SpriteFrames_method_get_frame_count:

.. rst-class:: classref-method

:ref:`int<class_int>` **get_frame_count** **(** :ref:`StringName<class_StringName>` anim **)** |const|

返回 ``anim`` 动画中的帧数。

.. rst-class:: classref-item-separator

----

.. _class_SpriteFrames_method_get_frame_duration:

.. rst-class:: classref-method

:ref:`float<class_float>` **get_frame_duration** **(** :ref:`StringName<class_StringName>` anim, :ref:`int<class_int>` idx **)** |const|

返回 ``anim`` 动画中 ``idx`` 帧的相对持续时间（默认为 ``1.0``\ ）。例如，持续时间为 ``2.0`` 的帧的显示长度是持续时间为 ``1.0`` 的帧的两倍。可以使用如下公式计算某一帧的绝对持续时间（单位为秒）：

::

    absolute_duration = relative_duration / (animation_fps * abs(playing_speed))

在这个例子中，\ ``playing_speed`` 是 :ref:`AnimatedSprite2D.get_playing_speed<class_AnimatedSprite2D_method_get_playing_speed>` 或 :ref:`AnimatedSprite3D.get_playing_speed<class_AnimatedSprite3D_method_get_playing_speed>`\ 。

.. rst-class:: classref-item-separator

----

.. _class_SpriteFrames_method_get_frame_texture:

.. rst-class:: classref-method

:ref:`Texture2D<class_Texture2D>` **get_frame_texture** **(** :ref:`StringName<class_StringName>` anim, :ref:`int<class_int>` idx **)** |const|

返回 ``anim`` 动画中帧索引为 ``idx`` 的纹理。

.. rst-class:: classref-item-separator

----

.. _class_SpriteFrames_method_has_animation:

.. rst-class:: classref-method

:ref:`bool<class_bool>` **has_animation** **(** :ref:`StringName<class_StringName>` anim **)** |const|

如果 ``anim`` 动画存在，则返回 ``true``\ 。

.. rst-class:: classref-item-separator

----

.. _class_SpriteFrames_method_remove_animation:

.. rst-class:: classref-method

void **remove_animation** **(** :ref:`StringName<class_StringName>` anim **)**

移除 ``anim`` 动画。

.. rst-class:: classref-item-separator

----

.. _class_SpriteFrames_method_remove_frame:

.. rst-class:: classref-method

void **remove_frame** **(** :ref:`StringName<class_StringName>` anim, :ref:`int<class_int>` idx **)**

移除 ``anim`` 动画中索引为 ``idx`` 的帧。

.. rst-class:: classref-item-separator

----

.. _class_SpriteFrames_method_rename_animation:

.. rst-class:: classref-method

void **rename_animation** **(** :ref:`StringName<class_StringName>` anim, :ref:`StringName<class_StringName>` newname **)**

将 ``anim`` 动画的名称更改为 ``newname``\ 。

.. rst-class:: classref-item-separator

----

.. _class_SpriteFrames_method_set_animation_loop:

.. rst-class:: classref-method

void **set_animation_loop** **(** :ref:`StringName<class_StringName>` anim, :ref:`bool<class_bool>` loop **)**

如果 ``loop`` 为 ``true``\ ，则 ``anim`` 动画会在到达结尾时循环，逆序播放时则为到达开头时循环。

.. rst-class:: classref-item-separator

----

.. _class_SpriteFrames_method_set_animation_speed:

.. rst-class:: classref-method

void **set_animation_speed** **(** :ref:`StringName<class_StringName>` anim, :ref:`float<class_float>` fps **)**

设置 ``anim`` 动画的速度，单位为帧每秒。

.. rst-class:: classref-item-separator

----

.. _class_SpriteFrames_method_set_frame:

.. rst-class:: classref-method

void **set_frame** **(** :ref:`StringName<class_StringName>` anim, :ref:`int<class_int>` idx, :ref:`Texture2D<class_Texture2D>` texture, :ref:`float<class_float>` duration=1.0 **)**

设置 ``anim`` 动画中索引为 ``idx`` 的帧的纹理 ``texture`` 和持续时间 ``duration``\ 。

.. |virtual| replace:: :abbr:`virtual (本方法通常需要用户覆盖才能生效。)`
.. |const| replace:: :abbr:`const (本方法没有副作用。不会修改该实例的任何成员变量。)`
.. |vararg| replace:: :abbr:`vararg (本方法除了在此处描述的参数外，还能够继续接受任意数量的参数。)`
.. |constructor| replace:: :abbr:`constructor (本方法用于构造某个类型。)`
.. |static| replace:: :abbr:`static (调用本方法无需实例，所以可以直接使用类名调用。)`
.. |operator| replace:: :abbr:`operator (本方法描述的是使用本类型作为左操作数的有效操作符。)`
.. |bitfield| replace:: :abbr:`BitField (这个值是由下列标志构成的位掩码整数。)`
