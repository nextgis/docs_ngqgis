.. sectionauthor:: Роман Гайнуллов <roman.gainullov@nextgis.ru>

.. _NextGIS_EasyQuery:

NextGIS EasyQuery
=================

Плагин NextGIS EasyQuery предназначен для быстрого поиска и фильтрации объектов векторных слоев.
Он является упрощенным и интуитивно понятным визуальным конструктором запросов, с помощью которого вы можете:

- Выбрать нужный векторный слой
- Задать простое условие для фильтрации объектов по атрибутивным данным
- Определить режим выборки
- Сохранить результат выборки в отдельный временный слой или выделить его в текущем векторном слое

Дополнительную информацию можно прочитать в разделе "О модуле"

.. figure:: _static/nextgis_easyquery/info.png
   :name: info
   :align: center
   :width: 16cm
   
   Информация о модуле

.. _ng_easyq_install:

Установка
---------

Для установки или обновления модуля необходимо найти его в меню Модули ‣ Управление модулями.
Введите часть или все его название в панель Поиск (см. :numref:`setup`).

.. figure:: _static/nextgis_easyquery/setup.png
   :name: setup
   :align: center
   :width: 16cm
   
   Список установленных и доступных к загрузке модулей

Выберите в списке NextGIS EasyQuery и выберите Установить модуль.

После установки расширения на панели инструментов появляется иконка |easyquery_icon|. 

.. |easyquery_icon| image:: _static/nextgis_easyquery/easyquery_icon.png

.. _ng_easyq_use:

Использование
-------------

1. Нажмите на иконку установленного плагина. Также открыть модуль можно через верхнее меню Вектор ‣ NextGIS EasyQuery
2. Выберите векторный слой, к объектам которого необходимо выполнить запрос. Слои в списке берутся из проекта, поэтому данные необходимо заранее добавить в QGIS.
3. Добавьте нужное вам условие - выберите поле для выборки, оператор и искомое значение. Условий может быть несколько, вы можете их добавлять и удалять.

.. figure:: _static/nextgis_easyquery/conditions.png
   :name: conditions
   :align: center
   :width: 25cm
   
   Добавление условия для выборки через плагин NextGIS EasyQuery
   
4. Установите режим выборки. Если вы задали несколько условий, то можете указать - должно выполниться хотя бы одно из них или все сразу.

.. figure:: _static/nextgis_easyquery/query_modes.png
   :name: query_modes
   :align: center
   :width: 16cm
   
   Выбор режима для выборки


.. important::
	Для числовых типов полей из списка будут предложены значения, соответствующие **процентным интервалам** 25, 50 и 75 %, а не все имеющиеся значения в текущем поле таблицы.

5. Выберите тип желаемого результата. Объекты могут быть как выделены в текущем слое, так и в сохранены в специальный временный слой.

.. figure:: _static/nextgis_easyquery/query_type_result.png
   :name: query_type_result
   :align: center
   :width: 16cm
   
   Выбор типа получаемого результата
   
6. По желанию установите флаг, чтобы результат выборки автоматически был приближен на карте.
7. Запустите выборку

.. figure:: _static/nextgis_easyquery/query_result.png
   :name: query_result
   :align: center
   :width: 25cm
   
   Результат выборки с выделением объектов в текущем слое


.. figure:: _static/nextgis_easyquery/query_result2.png
   :name: query_result2
   :align: center
   :width: 25cm
   
   Результат выборки с созданием нового временного слоя


Посмотрите на модуль в действии:

.. raw:: html

   <iframe width="560" height="315" src="https://rutube.ru/play/embed/4e972a2a1fbb40740efce482bdc299be/" frameBorder="0" allow="clipboard-write; autoplay" webkitAllowFullScreen mozallowfullscreen allowFullScreen></iframe>

Посмотреть видео на `youtube <https://youtu.be/VAZOQf2sUWg>`_, `rutube <https://rutube.ru/video/4e972a2a1fbb40740efce482bdc299be/>`_.
