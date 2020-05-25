.. sectionauthor:: Роман Гайнуллов <roman.gainullov@nextgis.ru>

.. _ngqgis_auth:

Авторизация в NextGIS QGIS
==========

Чтобы открыть дополнительные функциональные преимущества :program:`NextGIS QGIS` (перейти на Pro-версии NextGIS QGIS), 
необходимо приобрести план `Mini или Premium <http://nextgis.ru/nextgis-com/plans>`_ и авторизоваться в программе.

По умолчанию заблокированные инструменты показываются так: |blocked_tools| 
.. |blocked_tools| image:: _static/auth_ngqgis/blocked_tools.png

Для активации возможностей Pro-версии NextGIS QGIS необходимо авторизоваться в системе при помощи кнопки |not_auth|
NextGIS Account Toolbar на панели инструментов (см. :numref:`acc_toolbar_deactive`).
.. |not_auth| image:: _static/auth_ngqgis/not_auth.png

.. figure:: _static/auth_ngqgis/acc_toolbar_deactive.png
   :name: acc_toolbar_deactive
   :align: center
   :width: 10cm

   Общий вид NextGIS QGIS. NextGIS Account Toolbar деактивирован.
   
   
Авторизация происходит через веб-браузер с переадресацией на страницу https://my.nextgis.com/. 
На странице необходимо ввести данные вашего аккаунта NextGIS ID или пройти регистрацию (см. :numref:`auth_page`). 
Если вы забыли данные вашего аккаунта, то `восстановите <https://docs.nextgis.ru/docs_ngcom/source/faq_webgis.html#ngcom-change-passwords-webgis>`_ к нему доступ.

.. figure:: _static/auth_ngqgis/auth_page.png
   :name: auth_page
   :align: center
   :width: 10cm
   
   Страница авторизации NextGIS ID


После корректного указания пары логин/пароль вы получите сообщение об успешной авторизации в NextGIS QGIS (см. :numref:`suscess_auth.`), 
и доступ к Pro-функциям будет разблокирован |ublocked_tools.png|.
.. |unblocked_tools| image:: _static/auth_ngqgis/unblocked_tools.png

Кнопка NextGIS Account Toolbar при этом изменится на  |auth|, что говорит об успешно авторизованном пользователе (см. :numref:`acc_toolbar_active`).
.. |auth| image:: _static/auth_ngqgis/auth.png

.. figure:: _static/auth_ngqgis/suscess_auth.png
   :name: suscess_auth
   :align: center
   :width: 10cm
   
   Успешная авторизация в NextGIS QGIS

.. figure:: _static/auth_ngqgis/acc_toolbar_active.png
   :name: acc_toolbar_active
   :align: center
   :width: 10cm
   
   Общий вид NextGIS QGIS. NextGIS Account Toolbar активирован
