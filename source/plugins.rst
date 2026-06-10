

.. _ngqgis_plugins:
    
Модули расширения QGIS
============================

QGIS была разработана на архитектуре с поддержкой различных модулей, которые позволяют добавлять множество новых возможностей или функций в приложение. QGIS предоставляет библиотеки, которые могут использоваться для создания модулей. 
Большинство функций в QGIS реализованы как основные или внешние модули. Основные модули написаны на языках программирования C++ и Python. Все внешние модули в настоящее время написаны на языке Python. Они находятся во внешних репозиториях и поддерживаются написавшими их авторами. Внешние модули могут быть добавлены с помощью функции Установка модулей QGIS. 



Подробнее о модулях расширения можно почитать в следующих разделах:

.. toctree::
   :maxdepth: 1

   install_plugin
   update_plugins
   qms
   qconsolidate
   lesis2sqlite
   territory_plan_styler
   identifyplus
   easyquery
   digitizr
   molusce
   geom_paster
   osminfo
   clickfu
   dumploadfield
   qtiles
   connectpoints
   copycoords
   points2one
   joinlines
   multiqml
   quicksaveqml
   ogrstyle
   send2ge
   osmpoly_export
   shortcut
   reconstructline
   wurman_dots
   toolbox
   NextGIS Connect <https://docs.nextgis.ru/docs_ngconnect/source/index.html>
   Rosreestr tools <https://docs.nextgis.ru/docs_rosreestr_tools/source/index.html>



**Поддержка Qt6**

Постепенно добавляется поддержка Qt6. Модули, подходящие к установке в QGIS 4:

* MOLUSCE
* Geometry Paster
* OSMInfo
* QuickMapServices
* NextGIS Connect
* QGIS DevTools
* Wurman Dots
* QTiles
* Send2GE

Актуальный список модулей, поддерживающих Qt6, можно посмотреть `здесь <https://plugins.qgis.org/plugins/new_qgis_ready/>`_.
