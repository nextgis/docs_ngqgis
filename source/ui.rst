.. sectionauthor:: Дмитрий Барышников <dmitry.baryshnikov@nextgis.ru>

.. _ngqgis_ui:

Описание интерфейса NextGIS QGIS
=================================

При первом запуске :program:`NextGIS QGIS` пользователь видит следующее окно (см. :numref:`ngq_first_open`).

.. _ngq_fig_startup:

.. figure:: _static/UI_first_open_ru.png
   :name: ngq_first_open 
   :align: center
   :width: 20cm
   
   Первое открытие программы после установки
   
   В этом окне предлагается создать новый проект с нуля или при помощи шаблона. Также вы можете открыть уже существующий проект. 


.. figure:: _static/UI_main_ru.png
   :name: ngq_UIMainWindow 
   :align: center
   :width: 20cm

   Интерфейс :program:`NextGIS QGIS` с загруженным проектом

.. note::
   Внешний вид элементов интерфейса (заголовки окон и т.п.) может отличаться в 
   зависимости от операционной системы и менеджера окон.

Интерфейс :program:`NextGIS QGIS` разделяется на следующие области (см. :numref:`ngq_UIMainWindow`):

1. Главное меню.
2. Панель инструментов.
3. Браузер для просмотра папок
4. Дерево слоёв.
5. Область карты.
6. Панель NextGIS Connect
7. Панель поиска в QMS
8. Строка состояния.
9. Кнопка проекции.
10. Кнопка вызова панели отладочных сообщений.

.. _ngq_label_menubar:

Главное меню
------------------------------------

.. figure:: _static/UIMainWindowMenu_ru.png
   :name: ngq_UIMainWindowMenu
   :align: center
   :width: 20cm

   Главное меню NextGIS QGIS и выпадающее меню "Проект" 

Главное меню предоставляет доступ ко всем возможностям :program:`NextGIS QGIS` в 
виде стандартного иерархического меню. Рядом с пунктом меню указана иконка, соответствующая данному инструменту в панели инструментов, а также "горячие клавиши". Комбинации клавиш для пунктов меню заданы по умолчанию, но их можно изменить, вызвав диалог настройки из меню: :menuselection:``Установки ‣ Комбинации клавиш...``.

Несмотря на то, что большинству пунктов меню соответствует свой инструмент, меню 
и панели инструментов организованы по-разному. Дополнительную информацию 
об инструментах и панелях инструментов можно найти в разделе :ref:`ngq_label_toolbars`.

.. note::
   Дополнительные модули появляются в различных меню, поэтому на разных компьютерах 
   набор этих меню отличается.

.. _ngq_label_toolbars:

Панель инструментов
-------------------------------

.. figure:: _static/UIMainWindowButtons_ru.png
   :name: ngq_UIMainWindowButtons
   :align: center
   :width: 20cm

   Панель инструментов и всплывающая подсказка

Из панели инструментов можно запустить множество тех же самых функций, что и из меню, 
и ещё дополнительные инструменты для взаимодействия с картой. У каждой кнопки панели 
инструментов есть всплывающая подсказка: наведите мышку на соотвествующую кнопку, 
и на экране появится короткое описание ее функции.

Каждую панель инструментов можно передвигать по окну для ваших нужд. Панели можно 
скрывать и отображать при помощи контекстного меню, которое вызывается нажатием 
правой клавиши мыши на соответствующей панели.

.. _ngq_label_toolbars_on:

.. tip::

   В документации будут встречаться указания "Найдите кнопку на такой-то панели инструментов". 
   Для того чтобы найти конкретную панель инструментов, нажмите правой кнопкой мыши 
   на пустом участке панели инструментов. В контекстном меню выключите и включите 
   заданную панель, тогда вы увидите как она скрывается и показывается на экране.

.. _ngq_label_legend:

Дерево слоёв
----------------------------------

Понятие Слой будет часто встречаться в инструкции. Слой - это геоданные с определенным
составом и оформлением. Карта состоит из одного или нескольких слоев. Слои можно скрывать
и показывать. Можно изменять порядок расположения слоев и объединять их в группы.

.. figure:: _static/UIMainWindowLayers_ru.png
   :align: center
   :width: 20cm

   Дерево слоев

В дереве слоёв перечислены все слои открытого проекта. У каждого элемента есть флажок, который скрывает или показывает слой. Над деревом слоёв находится своя панель инструментов с командами: 

1. Открыть панель стиля слоя
2. Добавить группу слоёв
3. Управление темами карт (управляет видимостью слоя и темами)
4. Фильтровать легенду (по содержимому карты и личным слоям)
5. Фильтровать легенду по выражению
6. Развернуть все
7. Свернуть все
8. Удалить слой или группу

.. figure:: _static/layer_toobar_ru.png
   :align: center
   :width: 12cm

   Инструменты панели слоёв
   

Кнопка (3) позволяет добавить предустановку (preset), какие слои выключены, 
какие - включены. Это значит, что вы можете выбрать, какие слои на карте будут включены, 
и сохранить несколько таких настроек.  

Все эти предустановки так же видны из компоновщика карты. Вы можете составлять карты 
для печати на основе заданных вами комбинаций слоёв (см. :ref:`ngq_composer`).

Слой можно выделить мышью и перетащить выше или ниже других слоев для изменения 
порядка слоёв. Слой, находящийся сверху в списке, будет рисоваться на карте поверх других.

.. note::

   Это поведение может быть переопределено в панели ‘Порядок слоёв’.

Cлои в панели слоёв могут быть объединены в группы. Для этого есть два способа:

1. Нажать кнопку добавления новой группы (2). Ввести имя новой группы 
   и нажать ``Enter``. Нажать на существующий слой и перетащить его в группу.
2. Выделить несколько слоёв, нажать правой кнопкой в окне слоёв и выбрать 
   ``Сгруппировать выделенное``. (см. :numref:`UI_group_layers_context_pic`). Выделенные слои автоматически поместятся в новую группу. 

.. figure:: _static/UI_group_layers_context_ru.png
   :name: UI_group_layers_context_pic
   :align: center
   :width: 20cm
   
   Объединение слоёв в группу
   
Чтобы исключить слои из группы, перетащите их по дереву слоёв выше или ниже этой группы 
или кликните на них правой кнопкой и выберите ``Сделать элементом первого уровня``.

Группы могут быть вложены в другие группы.

Флажок возле имени группы даёт возможность переключать видимость всех слоев в группе 
одним действием.

Содержимое контекстного меню слоя, вызываемого правой кнопкой мыши, зависит от того, 
растровый это слой или векторный.

Вы можете выделять по несколько слоёв сразу, зажав клавишу ``Ctrl`` и нажимая на них 
левой клавишей мыши. Можно выделить несколько слоёв и сразу объединить их в новую 
группу. Можно выделить несколько слоёв и сразу удалить их из проекта, нажав ``Ctrl+D``. 
При этом файлы с жёсткого диска не удаляются.

.. _ngqgis_map_area:

Область карты
------------------

Это основное окно :program:`NextGIS QGIS` - тут отображается карта. Вид отображаемой
карты зависит от того, какие слои включены в панели слоёв, и какие им заданы стили. 

.. figure:: _static/UIMainWindowMap_ru.png
   :align: center
   :width: 20cm

   Основное окно NextGIS QGIS с отображенной картой

.. tip::
   **Масштабирование карты с помощью колеса мыши**

   Для изменения масштаба карты используйте колесо мыши. Поместите курсор на область карты и вращайте колесо. При этом карта отцентрируется на позиции курсора. Вы можете настроить поведение колеса мыши в меню ``Установки ‣ Параметры ‣ Инструменты ‣ Прокрутка и масштабирование``.

.. tip::
   **Перемещение карты, используя клавиши со стрелками и клавишу пробела**

   Вы можете поместить курсор мыши на карту и двигать карту клавишами со стрелками на клавиатуре. Так же можно зажать клавишу пробел или колесо мыши и двигать карту мышью.

.. _ngq_label_statusbar:

Строка состояния
-------------------

.. figure:: _static/UIMainWindowStatusbar_ru.png
   :align: center
   :width: 22cm

   Строка состояния

Слева находится окно поиска.

.. figure:: _static/UI_search_bar_ru.png
   :name: UI_search_bar_pic
   :align: center
   :width: 20cm
   
   Пример работы поиска

В строке состояния показывается позиция курсора на карте в текущих координатах 
(то есть метрах или градусах). Справа от окна координат есть кнопка с изображенем мыши, которая переключает показ между текущими координатами и охватом (bbox, extent).

Рядом с полем отображения координат находится список масштабов. В нём можно выбрать 
предустановленные масштабы от 1:500 to 1:1000000 или ввести точное значение с клавиатуры.

Далее расположено окно выбора увеличения. Если при изменении масштаба размер значков и толщина линий сохраняет своё значение в пикселях, то при выборе большего увеличения значки также увеличиваются визуально.

.. figure:: _static/Scale_vs_magnifier.png
   :name: Scale_vs_magnifier_pic
   :align: center
   :width: 20cm
   
   Один и тот же фрагмент карты при изменении масштаба (слева) и увеличения (справа)

Правее находится окно, в котором вы можете задать поворот карты 
в градусах по часовой стрелке.

Флажок ``Отрисовка`` при отключении остановит отрисовку карты. Если на экране 
открыто много тяжёлых слоёв, и отрисовка начинает тормозить, то можно временно выключить 
отрисовку, отключить лишние слои. 

Справа находится кнопка выбора проекции. На ней написан код :term:`EPSG` текущей системы координат. 
Если её нажать, то откроется окно свойств текущей проекции.

В правом углу находится кнопка вызова панели отладочных сообщений.

.. _ngqgis_map_elements:

Оформление карты
-------------------

В NextGIS QGIS имеется возможность отображать на карте элементы оформления.

* Масштабная линейка
* Координатная сетка
* Указатель на север
* Эмблема (картинка)
* Подпись авторских прав
* Название карты (с версии 3)
* Границы макета


.. figure:: _static/decorations.png
   :align: center
   :width: 16cm

   Карта с элементами оформления
   
Эти элементы оформления можно добавлять в 2 отдельных режимах:

* Для показа только в главном окне: меню Вид --> Оформление.
* Для вывода только на файлах и печать: в компоновщике карты.
