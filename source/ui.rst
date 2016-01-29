.. sectionauthor:: Дмитрий Барышников <dmitry.baryshnikov@nextgis.ru>

.. _ngqgis_ui:

********************************
Описание интерфейса |qg|
********************************




.. index::
   single:main window

При первом запуске |qg| пользователь видит окно, показанное ниже (номерами от 1 до 5 выделены пять основных областей, которые рассматриваются далее):


.. fixme:
   Заменить скриншот на |qg|


.. _fig_startup:


.. figure:: /_static/user_manual/introduction/startup.png
   :align: center
   :width: 35em

   Интерфейс |qg| с загруженным демонстрационным набором данных |nix|

.. note::
   Внешний вид элементов интерфейса (заголовки окон и т.п.) может отличаться, в зависисмости от операционной системы и менеджера окон.

Интерфейс |qg| разделяется на пять областей:

#. Главное меню
#. Панель инструментов
#. Дерево слоёв
#. Область карты
#. Строка состояния

Компоненты интерфейса |qg|, комбинации клавиш и контекстная справка более подробно описаны в следующих разделах

.. _label_menubar:

Главное меню
------------------------------------

.. index::
   single:menus


.. fixme:
   Тут вставить скрин всего окна |qg|, где главное меню отмечено красной рамкой.

Главное меню предоставляет доступ ко всем возможностям |qg| в виде стандартного иерархического меню. Ниже показаны меню верхнего уровня и краткое описание их содержимого, а также значки соответствующих им инструментов по мере их появления на панели инструментов и комбинации клавиш клавиатуры. Комбинации клавиш, описанные в этом разделе, заданы по умолчанию, но их можно изменить, вызвав диалог настройки из меню 
:menuselection:`Установки --> Комбинации клавиш...`.

Несмотря на то, что большинству пунктов меню соответствует свой инструмент, и наоборот, - меню и панели инструментов организованы по-разному. Панель инструментов, в которой находится инструмент, показана после каждого пункта меню в виде флажка.  Дополнительную информацию об инструментах и панелях инструментов можно найти в разделе :ref:`label_toolbars`.

.. note:
   Дополнительные модули появляются в различных меню, поэтому на разных компьютерах набор этих меню отличается.


.. fixme:
   Тут была большая таблица, просто со списком всех пунктов меню, я её пропустил из-за отсутствия смысла и трудоёмкости перевода.



.. _`label_toolbars`:

Панель инструментов
-------------------------------

.. index::
   single:toolbar


.. fixme:
   Тут вставить скрин всего окна |qg|, где панели инструментов отмечены красной рамкой.

Из панели инструментов можно запустить множество тех же самых функций, что и из меню, и ещё дополнительне инструменты для взаимодействия с картой. У каждой кнопки есть всплывающая подсказка - наведите мышку на кнопку, и на экране появится короткое описание.

Каждую панель инструментом можно передвигать по окну для ваших нужд. Панели можно включать-выключать, для этого наведите мышь на панель, нажмите правую кнопку, и у вас появится контекстное меню.


.. index::
   single:layout toolbars

.. fixme:
   уточнить названия меню



.. tip::
        **Восстановление панелей инструментов**

        Если вы нечаянно все панели, то их можно вернуть назад, используя пункт меню :menuselection:`Settings --> Toolbars -->`.

.. _`label_legend`:

Дерево слоёв
----------------------------------

Понятие **Слой** будет часто встречаться в инструкции. Слой - это то, что видно в дереве слоёв, технически это один файл, или одна таблица в БД. Их можно включать и выключать. Можно изменять порядок и объединять в группы.

.. fixme:
   Тут вставить скрин всего окна |qg|, где дерево слоёв отмечено красной рамкой.

.. index::
   single:legend

.. fixme:
   спросить, допустимо ли словосочетание "включает-выключает"

В дереве слоёв перечислены все слои открытого проекта. У каждого элемента есть флажок, который включает-выключает слой. Сверху дерева слоёв находится своя панель инструментов с коммандами: :guilabel:`Добавить группу слоёв`, :guilabel:`Управление видимости слоя`, :guilabel:`Фильтровать легенду по содержимому карты`, :guilabel:`Развернуть все`, :guilabel:`Свернуть все`, :guilabel:`Удалить слой или группу`.

.. _figure_layer_toolbar:

.. only:: html

   **Figure Layer tools Bar:**

   .. figure:: /_static/user_manual/introduction/layer_toobar.png
      :align: center

      Панель инструментов в дереве слоёв |nix|

Кнопка |mActionShowPresets| позволяет добавить предустановку (preset) какие слои выключены, какие - включены. Это значит, что вы можете выбрать, какие слои на карте будут включены, и сохранить несколько таких настроек.  To add a preset view just click on |mActionShowPresets|, choose *Add Preset...* from the drop down menu and give a name to the preset. After that you will see a list with all the presets that you can recall pressing on the |mActionShowPresets| button. 


Все эти предустановки так же видны из компоновщика карты. Вы можете составлять карты для печати на основе заданных вами комбинаций слоёв (см. :ref:`composer_main_properties`).



.. index::
   single:layer visibility

Слой можно выделить мышью и перетащить вверх или вниз для изменения порядка слоёв. Слой находящийся сверху в списке будет рисоваться на карте поверх других.

.. note::

   Это поведение может быть переопределено в панели ‘Layer order’.

Cлои в панели слоёв могут быть объединены в группы. Для этого есть два способа:

#. Нажать кнопку добавления новой группы |mActionFolder|. Ввести имя новой группы и нажать :kbd:`Enter`. Нажать на существующий слой и перетащить его в группу.
#. Выделить несколько слоёв, нажать правой кнопкой в окне слоёв, и выбрать :guilabel:`Сгруппировать выделенное`. Выбранные слои автоматически поместятся в новую группу. 

Что бы вынести слои из группы, перетащите их по дереву слоёв выше или ниже этой группы, или нажмите правой кнопкой на них и выберите :guilabel:`Сделать элементом первого уровня`.

Группы могут быть вложены в другие группы.

Флажок возле имени группы даёт возможность переключать видимость всех слоев в группе одним действием.

Содержимое контекстного меню слоя, вызываемого правой кнопкой мыши, зависит от того, растровый это слой, или векторный.

.. fixme:
   Тут был список кнопок меню **Right mouse button menu for raster layers**, я его выкинул, потому что от него толка нет.

Вы можете выделять по несколько слоёв сразу, зажав :kbd:`Ctrl` и нажимая на них левой клавишей мыши. Можно выделить несколько слоёв и сразу объединить их в новую группу. Можно выделить несколько слоёв и сразу удалить из из проекта, нажав :kbd:`Ctrl+D`. Удаляются слои из проекта, а их файлы с жёсткого диска - не удаляются.

Working with the Legend independent layer order
...............................................

There is a panel that allows you to define an independent drawing order for the map legend.
You can activate it in the menu :menuselection:`Settings --> Panels --> Layer
order`. This feature allows you to, for instance, order your layers in order of importance,
but still display them in the correct order (see figure_layer_order_).
Checking the |checkbox| :guilabel:`Control rendering order` box underneath the
list of layers will cause a revert to default behavior.

.. _figure_layer_order:

.. only:: html

   **Figure Layer Order:**

.. figure:: /_static/user_manual/introduction/layer_order.png
    :align: center

    Define a legend independent layer order |nix|

.. _`label_mapview`:

Map View
--------

.. index::`map view`

This is the "business end" of |qg| --- maps are displayed in this area! The
map displayed in this window will depend on the vector and raster layers you
have chosen to load (see sections that follow for more information on how to
load layers). The map view can be panned, shifting the focus of the map display
to another region, and it can be zoomed in and out. Various other operations can be
performed on the map as described in the toolbar description above. The map
view and the legend are tightly bound to each other --- the maps in view reflect
changes you make in the legend area.

.. index::
   single:zoom mouse wheel

.. tip::
   **Zooming the Map with the Mouse Wheel**

   You can use the mouse wheel to zoom in and out on the map. Place the mouse
   cursor inside the map area and roll the wheel forward (away from you) to
   zoom in and backwards (towards you) to zoom out. The zoom is centered on the
   mouse cursor position. You can customize the behavior of the
   mouse wheel zoom using the :guilabel:`Map tools` tab under the
   :menuselection:`Settings --> Options` menu.

.. tip::
   **Panning the Map with the Arrow Keys and Space Bar**

   .. index::
      single:pan arrow keys

   You can use the arrow keys to pan the map. Place the mouse cursor inside
   the map area and click on the right arrow key to pan east, left arrow key to
   pan west, up arrow key to pan north and down arrow key to pan south. You can
   also pan the map using the space bar or the click on mouse wheel: just move
   the mouse while holding down space bar or click on mouse wheel.

.. _`label_mapoverview`:


.. _`label_statusbar`:

Status Bar
----------

The status bar shows you your current position in map coordinates (e.g.,
meters or decimal degrees) as the mouse pointer is moved across the map view.
To the left of the coordinate display in the status bar is a small button that
will toggle between showing coordinate position or the view extents of the
map view as you pan and zoom in and out.

Next to the coordinate display you will find the scale display. It shows the scale of
the map view. If you zoom in or out, |qg| shows you the current scale. There is
a scale selector, which allows you to choose between predefined scales from
1:500 to 1:1000000.

To the right of the scale display you can define a current clockwise rotation for
your map view in degrees.

A progress bar in the status bar shows the progress of rendering as each layer is
drawn to the map view. In some cases, such as the gathering of statistics in
raster layers, the progress bar will be used to show the status of lengthy
operations.

If a new plugin or a plugin update is available, you will see a message at the
far left of the status bar. On the right side of the status bar, there is a small
checkbox which can be used to temporarily prevent layers being rendered to the
map view (see section :ref:`redraw_events` below). The icon |mIconStopRendering|
immediately stops the current map rendering process.

To the right of the render functions, you find the EPSG code of the current
project CRS and a projector icon. Clicking on this opens the projection
properties for the current project.


.. tip::
   **Calculating the Correct Scale of Your Map Canvas**

   .. index::
      single:scale calculate

   When you start |qg|, the default units are degrees, and this means that |qg| will interpret any
   coordinate in your layer as specified in degrees. To get correct scale values, you can
   either change this setting to meters manually in the :guilabel:`General` tab
   under :menuselection:`Settings --> Project Properties`, or you can select a
   project CRS clicking on the |mIconProjectionDisabled| :sup:`Current CRS:` icon in the
   lower right-hand corner of the status bar. In the last case, the units are set to what the
   project projection specifies (e.g., '+units=m').

