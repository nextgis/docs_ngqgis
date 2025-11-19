


Установка и обновление
=======================

Для установки :program:`NextGIS QGIS` используется универсальный сетевой установщик, который можно скачать `по ссылке <http://nextgis.ru/nextgis-qgis/>`_ или **Flatpak** для операционных систем Linux. В личном кабинете также доступен `оффлайн-инсталлятор <https://my.nextgis.com/software>`_.

Ниже приведены инструкции по установке для операционных систем `Windows <https://docs.nextgis.ru/docs_ngqgis/source/install.html#windows>`_ и `Linux <https://docs.nextgis.ru/docs_ngqgis/source/install.html#linux>`_.

.. _windows:

Windows
--------

.. _ngqgis_sys_req:

Системные требования 
^^^^^^^^^^^^^^^^^^^^

Минимальные параметры ПК
~~~~~~~~~~~~~~~~~~~~~~~~~

* ОС Windows 7 и выше, 64 бит
* процессор Intel Core i3 с тактовой частотой не менее 2 ГГц (2 ядра) или аналог
* оперативная память не менее 4 ГиБ
* соответствующая материнская плата для выбранных процессоров со встроенной видеокартой
* накопитель на жестких магнитных дисках емкостью не менее 40 ГБ
* манипулятор “мышь”
* клавиатура
* монитор LCD 14”, разрешение 1024х768

Рекомендуемые параметры ПК
~~~~~~~~~~~~~~~~~~~~~~~~~~

* ОС Windows 10 и выше, 64 бит
* процессор Intel Core i5 с тактовой частотой не менее 2.8 ГГц (4 ядра) или аналог
* оперативная память не менее 16 ГиБ
* соответствующая материнская плата для выбранных процессоров 
* дискретная видеокарта с объемом видео памяти не менее 4 ГиБ
* накопитель на жестких магнитных дисках или SSD емкостью не менее 500 ГБ
* манипулятор “мышь”
* клавиатура
* источник бесперебойного питания емкостью не менее 800 ВА
* монитор LCD 24”, разрешение 2560x1440



.. _ngqgis_install:

Установка на Windows
^^^^^^^^^^^^^^^^^^^^^

Установщик представляет собой пошаговый мастер. Первая страница мастера содержит приглашение к началу установки.

.. figure:: _static/install_wizard_welcome_ru.png
   :name: ngqgis_installPage01
   :align: center
   :width: 16cm

   Начальная страница мастера установки

На второй странице необходимо указать путь до папки установки. Рекомендуется оставить предложенный мастером путь.

.. figure:: _static/install_wizard_path_ru.png
   :name: ngqgis_installPage02
   :align: center
   :width: 16cm

   Выбор папки для установки

На третьей странице можно отключить некоторые компоненты, если они не нужны при работе.

.. figure:: _static/install_wizard_components_ru.png
   :name: ngqgis_installPage03
   :align: center
   :width: 16cm

   Выбор компонентов для установки

На четвертой странице мастера необходимо прочитать и принять лицензионное соглашение.

.. figure:: _static/install_wizard_license_ru.png
   :name: ngqgis_installPage04
   :align: center
   :width: 16cm
   
   Страница лицензионного соглашения в мастере установки

На пятой странице необходимо указать имя для папки в меню "Пуск".

.. figure:: _static/install_wizard_start_folder_ru.png
   :name: ngqgis_installPage05
   :align: center
   :width: 16cm

   Выбор папки в меню "Пуск"

На шестой странице мастер сообщит о готовности начать установку. 

.. figure:: _static/install_wizard_ready_ru.png
   :name: ngqgis_installPage06
   :align: center
   :width: 16cm

   Шестая страница мастера установки
   
После нажатия кнопки **Установить** начнётся процесс распаковки и установки файлов.
По окончании этого процесса появится финальное окно с сообщением об успешной установки программы.


.. _ngqgis_update:

Обновление на Windows
^^^^^^^^^^^^^^^^^^^^^

.. _ngqgis_update_check:

Как проверить текущую версию программы
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Запустите NextGIS QGIS и перейдите в ``Справка  ‣ О программе``.

.. figure:: _static/ngq_check_version_en.png
   :name: ngq_check_version_pic
   :align: center
   :width: 10cm

   Проверка установленной версии NextGIS QGIS

* Если ваша версия 24.\* и выше, перейдите к `проверке обновлений <https://docs.nextgis.ru/docs_ngqgis/source/install.html#ngqgis-upadate-24up>`_.
* Если ваша версия 23.\* и ниже, необходимо выполнить `полное удаление программы и повторную установку <https://docs.nextgis.ru/docs_ngqgis/source/install.html#ngqgis-update-23>`_ свежего дистрибутива.

.. _ngqgis_update_23:

Если у вас установлена версия 23 и ниже
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Для полного удаления программы перейдите в ваш список установленных приложений и найдите NextGIS Maintenance Tool или Сервисный режим NextGIS.

.. figure:: _static/ngq_maint_select_ru.png
   :name: ngq_maint_select_pic
   :align: center
   :width: 8cm

   Сервисный режим NextGIS в списке приложений

Выберите *Удаление всех компонентов* и нажмите **Далее**. 

.. figure:: _static/ngq_delete_ru.png
   :name: ngq_delete_pic
   :align: center
   :width: 16cm

   Удаление старой версии

Для подтверждения удаления нажмите **Удалить**.

.. figure:: _static/ngq_delete_finish_ru.png
   :name: ngq_delete_finish_pic
   :align: center
   :width: 16cm


После завершения установки нажмите **Выйти**.

Загрузите актуальный дистрибутив в `личном кабинете <http://my.nextgis.com/software>`_ или на `nextgis.ru <https://nextgis.ru/nextgis-qgis/>`_ по кнопке **Скачать ознакомительную версию**.

Запустите скачанный дистрибутив и пройдите по `шагам установки <https://docs.nextgis.ru/docs_ngqgis/source/install.html#ngqgis-install>`_

.. _ngqgis_update_24up:

Если ваша версия 24.\* и выше
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Выполните проверку обновлений.
Для этого запустите NextGIS QGIS и перейдите в ``Справка - Проверить версию QGIS``.

.. figure:: _static/ngq_check_updates_ru.png
   :name: ngq_check_updates_pic
   :align: center
   :width: 10cm

   Проверка версии QGIS из меню "Справка"

В программе появится уведомление о доступном обновлении. Нажмите **Обновить**. Если у вас последняя версия, появится сообщение "Нет доступных обновлений".

Откроется Сервисный режим NextGIS, нажмите **Далее**.

.. figure:: _static/ngq_maint_update_ru.png
   :name: ngq_maint_update_pic
   :align: center
   :width: 16cm

   Выбор обновления компонентов

Выполнится поиск и установка обновлений. 
После завершения установки нажмите **Выйти**.



.. _linux:

Linux
-----

.. _ngqgis_install_linux:

Установка на Linux
^^^^^^^^^^^^^^^^^^

Актуальным способом распространения NextGIS QGIS в Linux сейчас является Flatpak. У нас развёрнут репозиторий по адресу flatpak.nextgis.com. Данная инструкция описывает установку и обновление при наличии доступа в интернет. 

1. Установка Flatpak

Установите Flatpak способом, используемым в вашей ОС: 


* `ALT Linux <https://www.altlinux.org/Flatpak>`_
* `РЕД ОС <https://redos.red-soft.ru/base/redos-7_3/7_3-administation/7_3-isolated-env/7_3-flatpak/>`_
* `Astra Linux <https://wiki.astralinux.ru/kb/osnovy-ispol-zovaniya-flatpak-205885327.html>`_ (требуется аккаунт для доступа)
* Другие ОС можно найти в `списке <https://flathub.org/ru/setup>`_


2. Установка NextGIS QGIS

Самый простой способ установки — использовать файл com.nextgis.ngqgis.flatpakref.
Его можно открыть в графическом установщике или передать как аргумент команде flatpak install

.. _install_linux_graph:

Установка с помощью графического интерфейса
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

#. Скачайте файл `com.nextgis.ngqgis.flatpakref <https://flatpak.nextgis.com/repo/appstream/com.nextgis.ngqgis.flatpakref>`_
#. Откройте файловый менеджер и перейдите в каталог загрузок
#. Откройте com.nextgis.ngqgis.flatpakref в графическом установщике, например, KDE Discover (в окружении KDE) или Gnome Software (в окружении Gnome)
#. Нажмите **установить**

.. figure:: _static/flatpak_graphic_ru.png
   :name: 
   :align: center
   :width: 20cm

.. _install_linux_terminal:

Установка с помощью терминала
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Откройте терминал и выполните команду

.. code-block::

   flatpak install https://flatpak.nextgis.com/repo/appstream/com.nextgis.ngqgis.flatpakref


В процессе будет предложено добавить репозитории NextGIS и Flathub, если они ещё не были настроены.

Вы также можете установить NextGIS QGIS только для текущего пользователя, если это требуется для рабочего процесса. Для этого передайте флаг --user в команду install:

.. code-block::

   flatpak install --user https://flatpak.nextgis.com/repo/appstream/com.nextgis.ngqgis.flatpakref

.. _ngqgis_update_linux:

Обновление на Linux
^^^^^^^^^^^^^^^^^^-

Если у вас ранее была установлена оффлайн-версия NextGIS QGIS, предварительно нужно её удалить с помощью команды flatpak uninstall com.nextgis.ngqgis, и выполнить установку по инструкции выше. 

.. _update_linux_graph:

Обновление с помощью графического интерфейса
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

#. Откройте KDE Discover (в окружении KDE) или Gnome Software (в окружении Gnome)
#. В поиске введите NextGIS QGIS
#. Нажмите кнопку **Обновить**

.. _update_linux_terminal:

Обновление с помощью терминала
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Откройте терминал и выполните команду

.. code-block::

   flatpak update com.nextgis.ngqgis


