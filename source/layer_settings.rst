

.. _ngmobile_layer_settings:

Настройки слоев
===============

Карта представляет собой набор растровых и векторных слоев. Панель дерева слоев отражает содержимое карты и позволяет контролировать видимость и порядок слоев.

Для переключения видимости слоя следует нажать на кнопку |ic_eye|.

Настройки слоя можно открыть из `контекстного меню <https://docs.nextgis.ru/docs_ngmobile/source/main.html#ngmob-layer-menu>`_.

В настройках есть следующие вкладки:

* `Общие <https://docs.nextgis.ru/docs_ngmobile/source/layer_settings.html#ngmobile-tab-general-settings>`_ - для всех типов слоёв;
* `Стиль <https://docs.nextgis.ru/docs_ngmobile/source/layer_settings.html#ngmobile-style-settings>`_ - для векторных слоёв;
* `Кэш <https://docs.nextgis.ru/docs_ngmobile/source/layer_settings.html#ngmobile-cache-settings>`_ - для векторных слоёв, здесь можно перестроить кэш.

.. _ngmobile_tab_general_settings:

Общие настройки
---------------

Блок настроек "Общие" показывает такую информацию о слое:

* Локальный путь - где файл лежит на устройстве и как точно называется.
* Имя слоя - можно настроить имя, под которым слой отображается на карте.
* Масштабные уровни, на которых слой виден на карте. По умолчанию стоит полный диапазон - от 0 до 25 уровня зума. Можно настроить видимость слоя только на определенных масштабных уровнях.

.. figure:: _static/style_vector_general_ru.png
   :name: ngmobile_style_vector_general_pic
   :align: center
   :width: 10cm
   
   Общие настройки векторного слоя

.. figure:: _static/style_raster_general_ru.png
   :name: ngmobile_style_raster_general_pic
   :align: center
   :width: 10cm
   
   Общие настройки растрового слоя

.. _ngmobile_vector_layer_settings:
.. _ngmobile_style_settings:

Настройки стиля векторного слоя
-------------------------------

При выборе пункта "Настройки" в контекстном меню слоя открывается окно настроек векторного слоя. 

Доступные настройки стиля векторного слоя зависят от типа геометрии слоя и выбранного типа **отрисовки** - `обычной <https://docs.nextgis.ru/docs_ngmobile/source/layer_settings.html#ngmobile-simple-rendering>`_ или `по правилу <https://docs.nextgis.ru/docs_ngmobile/source/layer_settings.html#ngmobile-rule-rendering>`_.

.. _ngmobile_simple_rendering:

Обычная отрисовка
~~~~~~~~~~~~~~~~~

При обычной отрисовке все объекты слоя будут иметь одинаковую форму, цвет, размер и т.д.

Для слоя с любой геометрией можно настроить:

* Цвет заливки;
* Цвет обводки;
* Толщину обводки;
* Подписи.

Также есть настройки, специфические для определённого типа геометрии: 

Например, для слоев с |ic_type_multipoint| **точечной/мультиточечной** геометрией можно установить размер пунсона (кружка).

.. figure:: _static/style_vector_point_settings_ru.png
   :name: style_vector_point_settings_pic
   :align: center
   :width: 10cm
   
   Настройки стиля точечного векторного слоя

.. figure:: _static/style_vector_point_result_ru.png
   :name: style_vector_point_result_pic
   :align: center
   :width: 10cm

   Два точечных слоя с разным размером пунсона

Для слоев с |ic_type_line| **линейной/мультилинейной** геометрией можно задать тип линии:

* сплошная - учитывается только цвет заливки;
* пунктир - учитывается только цвет заливки;
* сплошная по границам - учитывается и цвет заливки, и цвет обводки.

.. figure:: _static/style_vector_line_settings_ru.png
   :name: style_vector_line_settings_pic
   :align: center
   :width: 10cm

   Настройки стиля линейного слоя

.. figure:: _static/style_vector_line_result_ru.png
   :name: style_vector_line_result_pic
   :align: center
   :width: 10cm

   Линейные слои с разными типами линии: "пунктир" и "сплошная по границам"

Для слоев с |ic_type_polygon| **полигональной/мультиполигональной** геометрией можно выбрать/отменить опцию заливки полигона. Заливка полигона, когда она включена, полупрозрачная.

.. figure:: _static/style_vector_polygon_settings_ru.png
   :name: style_vector_polygon_settings_pic
   :align: center
   :width: 10cm

   Настройки стиля полигонального слоя

.. figure:: _static/style_vector_polygon_result_ru.png
   :name: style_vector_polygon_result_pic
   :align: center
   :width: 10cm

   Полигональные слои с заливкой и без

.. _ngmob_labels:

Подписи
~~~~~~~~

Для слоев с любой геометрией также можно выбрать опцию показа подписей каждого объекта на карте. 

Через контекстное меню слоя зайдите в Настройки. На вкладке Стиль поставьте флажок напротив пункта **Подпись**.

Есть два варианта подписей:

* Индивидуальные для каждого объекта, значение берётся из выбранного поля.
* Одинаковые для всех объектов - просто введите текст в поле.

Поле, выбранное для подписей объектов на карте, может не совпадать с полем, значение которого используется в качестве `идентификатора при выделении объекта <https://docs.nextgis.ru/docs_ngmobile/source/layer_settings.html#ngmobile-fields-settings>`_.

.. figure:: _static/label_vs_feature_name_ru.png
   :name: label_vs_feature_name_pic
   :align: center
   :width: 10cm

   1 - идентификатор выделенного объекта и название слоя, 2 - подпись объекта на карте

.. _ngmobile_rule_rendering:

Отрисовка по правилу
~~~~~~~~~~~~~~~~~~~~

Можно выбрать отрисовку по правилу для векторного слоя и задать разные типы форм, цвета, размера и т.д. для объектов слоя в зависимости от их атрибутов.

Для этого следует выбрать отрисовку по правилу, что приведет к открытию других настроек стиля (см. :numref:`ngmobile_style_vector_rulebased_pic`).

.. figure:: _static/style_vector_rulebased.png
   :name: ngmobile_style_vector_rulebased_pic
   :align: center
   :width: 10cm
   
   Настройки стиля векторного слоя (стиль отрисовки по правилу).
   
   Цифрами обозначено: 1 - тип отрисовки; 2 - выбор поля атрибутов; 3 - ранее созданные правила; 4 - кнопка "Создать новое правило"; 5 - кнопка "Удалить правило".
   
Для начала следует выбрать поле атрибутов, по значению которого будут созданы правила (см. :numref:`ngmobile_style_vector_rulebased_pic`, п.2). 

Затем необходимо нажать на кнопку "Создать новое правило" (см. :numref:`ngmobile_style_vector_rulebased_pic`, п.4), что приведет к открытию списка уникальных значений поля атрибутов, выбранного ранее. Следует выбрать значение и нажать "ОК", чтобы открыть диалог настроек стиля (см. :numref:`ngmobile_style_vector_rulebased_item_pic`).

.. figure:: _static/style_vector_rulebased_item.png
   :name: ngmobile_style_vector_rulebased_item_pic
   :align: center
   :width: 10cm
   
   Диалог настроек стиля с отрисовкой по правилу.
   
В данном диалоге можно выбрать и применить те же настройки, которые были описаны выше в разделе :ref:`ngmobile_simple_rendering` (настройки стиля с отрисовкой по правилу также зависят от типа векторного слоя). Когда все настройки будут заданы, следует нажать "OK". 

Так можно создать стили с отрисовкой по правилу для каждого значения выбранного поля атрибутов.

.. _ngmobile_fields_settings:

Поля
----

В данном блоке настроек можно выбрать поле атрибутов, которое будет использоваться как ID объекта при редактировании.

.. figure:: _static/style_select_field.png
   :name: ngmobile_style_select_field_pic
   :align: center
   :width: 10cm
   
   Блок настроек векторного слоя "Поля".

.. warning::
   Выбранное поле не будет использовано для подписей на карте, подробнее о настройках подписей в разделе :ref:`ngmobile_style_settings`.

.. _ngmobile_cache_settings:

Настройки кэша
--------------

Используя блок настроек "Кэш", можно выполнить перестроение кэша для оптимизации
процессов создания слоя с возможностью сохранения и отмены внесенных изменений.



.. seealso:: Посмотрите, как настроить кэш растрового слоя, в видео:

.. raw:: html

   <iframe width="560" height="315" src="https://rutube.ru/play/embed/93d74bd3bf13314d6a40d37fe1a62060/" frameBorder="0" allow="clipboard-write; autoplay" webkitAllowFullScreen mozallowfullscreen allowFullScreen></iframe>

Посмотреть видео на `youtube <https://youtu.be/9g4GrdlkaRI>`_, `rutube <https://rutube.ru/video/93d74bd3bf13314d6a40d37fe1a62060/>`_.

.. |ic_eye| image:: _static/ic_eye.png
   :width: 7mm
   :alt: глаз

.. |ic_type_multipoint| image:: _static/ic_type_multipoint.png
   :width: 7mm
   :alt: глаз

.. |ic_type_polygon| image:: _static/ic_type_polygon.png
   :width: 7mm
   :alt: глаз

.. |ic_type_line| image:: _static/ic_type_line.png
   :width: 7mm
   :alt: глаз






