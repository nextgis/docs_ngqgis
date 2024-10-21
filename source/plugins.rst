.. sectionauthor:: Дмитрий Барышников <dmitry.baryshnikov@nextgis.ru>

.. _ngqgis_plugins:
    
Модули расширения
=================

QGIS была разработана на архитектуре с поддержкой различных модулей, которые позволяют 
добавлять множество новых возможностей или функций в приложение. QGIS предоставляет 
библиотеки, которые могут использоваться для создания модулей. 
Большинство функций в QGIS реализованы как основные или внешние модули. 
Основные модули написаны на языках программирования C++ и Python.
Все внешние модули в настоящее время написаны на языке Python. Они находятся во 
внешних репозиториях и поддерживаются написавшими их авторами. Внешние модули могут 
быть добавлены с помощью функции Установка модулей QGIS. 

.. _ngqgis_plugins_install:

Установка плагинов
-------------------------

Вам потребуется подключение к сети. 

Для установки и обновления плагинов необходимо нажать :menuselection:`Модули --> Управление модулями`.

Если вам надо установить плагин, введите часть его названия в панель Поиск. 


.. figure:: _static/modules_control.png
   :align: center
   :width: 16cm
   
   Список установленных и доступных к загрузке модулей.

Выберите в списке нужный модуль и нажмите кнопку Установить модуль. 

Модули могут быть установленными, но не включёнными: если в списке у модуля не установлен 
флажок, то он не будет загружаться. Активируются модули автоматически с помощью 
установки флажка на соответствующем модуле.

Если вы ввели название модуля правильно, а модуля, который нужно установить, не нашли, 
то выполните следующие операции:

1. Проверьте вкладку Параметры: у репозиториев должна быть зелёная отметка. Если 
   отметка красная, значит проблемы либо в подключении к интернету, либо с сервером.
2. Попробуйте установить флажок для активации пункта Разрешить установку экспериментальных модулей.
3. Проверьте, нужный модуль может находиться в каком-то специальном репозитории, 
   спросите у того, кто вам про него сказал. 

.. _ngqgis_plugins_descr:

Описание модулей расширения
=====================================

Подробнее о модулях расширения можно почитать в следующих разделах:

* `NextGIS Connect <https://docs.nextgis.ru/docs_ngconnect/source/toc.html>`_
* `Rosreestr Tools <https://docs.nextgis.ru/docs_rosreestr_tools/source/toc.html>`_

* `QuickMapServices <https://docs.nextgis.ru/docs_ngqgis/source/qms.html>`_
* `QConsolidate <https://docs.nextgis.ru/docs_ngqgis/source/qconsolidate.html>`_
* `Привязка растров <https://docs.nextgis.ru/docs_ngqgis/source/raster_ref.html>`_
* `Lesis2SQLite <https://docs.nextgis.ru/docs_ngqgis/source/lesis2sqlite.html>`_
* `Territory Plan Styler <https://docs.nextgis.ru/docs_ngqgis/source/territory_plan_styler.html>`_
* `IdentifyPlus <https://docs.nextgis.ru/docs_ngqgis/source/identifyplus.html>`_
* `NextGIS EasyQuery <https://docs.nextgis.ru/docs_ngqgis/source/easyquery.html>`_
* `Digitizr <https://docs.nextgis.ru/docs_ngqgis/source/digitizr.html>`_
* `MOLUSCE 4.0 <https://docs.nextgis.ru/docs_ngqgis/source/molusce.html>`_
* `Geometry Paster <https://docs.nextgis.ru/docs_ngqgis/source/geom_paster.html>`_


.. to do::
   :maxdepth: 2

   qms
   plugin_rectangles_ovals_digitizing
   qconsolidate
   raster_ref
   lesis2sqlite
   territory_plan_styler
   identifyplus
   easyquery
   digitizr
   molusce
   geom_paster
   
