OSMPoly_export
===============

Модуль позволяет экспортировать объекты мультиполигонального слоя или слой целиком в poly-формате.

Такие файлы открываются в редакторе данных OpenStreetMap – JOSM.

После установки модуль появится в панели инструментов работы с векторными данными: |button_osmpoly|.

.. |button_osmpoly| image:: _static/button_osmpoly.png
   :width: 6mm

* Выберите нужный слой в панели слоёв QGIS.

* Выделите объекты, которые хотите сконвертировать. Активируйте модуль.

.. note:: Если не выделить объекты, будут сконвертированы все, о чём появится предупреждающее сообщение.

* Во всплывающем окне модуля выберите текстовое поле, из которого будут взяты названия для poly-файлов.

.. figure:: _static/select_name_field_ru.png
   :name: select_name_field_pic
   :align: center
   :width: 6cm

   Выбор поля названия

* Укажите путь к целевой папке.

Каждый полигон слоя сохранится отдельным poly-файлом.

Посмотрите, как работать с модулем, в нашем `видео <https://youtu.be/q_5I5RZsOi4>`_.
