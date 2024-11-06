ReconstructLine
================

Модуль позволяет cоздавать линии из точек.

Точки могут быть неупорядоченными по времени и другим атрибутам, но учитывается пространственное расположение точек.

После установки кнопки модуля появятся на панели инструментов.

.. |button_copy_points| image:: _static/button_copy_points.png
   :width: 6mm

.. |button_paste_line| image:: _static/button_paste_line.png
   :width: 6mm

.. |button_paste_fragments| image:: _static/button_paste_fragments.png
   :width: 6mm


* Выделите слой.

* Выделите точки, из которых хотите создать линию.

* Нажмите **Скопировать точки** |button_copy_points|.

* Выберите линейный слой, в который хотите добавить линию. Переведите его в режим редактирования.

* Нажмите **Вставить линию** |button_paste_line| или **Вставить составную линию** |button_paste_fragments|.

* В следующем окне введите атрибуты объектов.

.. figure:: _static/paste_line_attr_ru.png
   :name: 
   :align: center
   :width: 6cm

   Ввод значений атрибутов линии

Для аналогичного соединения точек по значению в таблице атрибутов используйте модуль `Points2One <https://docs.nextgis.ru/docs_ngqgis/source/points2one.html>`_.
