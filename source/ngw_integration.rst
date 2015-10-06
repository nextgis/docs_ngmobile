.. sectionauthor::  Наталья Барышникова <Nshelekhova@gmail.com>

.. _ngmob_integration:


Интеграция с NextGIS Web
========================

С основными возможностями программного обеспечения NextGIS Web можно ознакомиться 
в подразделе :ref:`ngweb_keyfeatures`.

Создание подключения к NextGIS Web
-----------------------------------

Подключение к программному обеспечению NextGIS Web может осуществляться несколькими 
способами. При использовании **первого способа** подключения к NextGIS Web, необходимо 
выполнить следующую последовательность шагов:

1. Вызвать меню опций (см. :numref:`ngmobile_main_activity_pic` п. 5). 
2. Далее выбрать пункт меню "Добавить слой".
3. В открывшемся меню опций необходимо выбрать пункт "NGW" (см. :numref:`ngmobile_add_ngw_layer_pic`) 

.. figure:: _static/add_layer1.png
   :name: ngmobile_add_ngw_layer_pic
   :align: center
   :height: 10cm
  
   Добавление слоя NextGIS Web

4. В открывшемся окне необходимо выбрать "Добавить учетную запись" (Добавить учетную запись NextGIS Web). 
   Нажать на эту кнопку (см. :numref:`ngmobile_select_ngw_layer_pic`).

.. figure:: _static/select_layer.png
   :name: ngmobile_select_ngw_layer_pic
   :align: center
   :height: 10cm
   
   Добавление учетной записи NextGIS Web

5. В открывшемся окне надо ввести параметры подключения: NextGIS Web :term:`URL`, 
   Имя пользователя/логин и пароль, нажать кнопку "Подключить" 
   (см. :numref:`ngmobile_ngw_connection_settings_pic`).

.. figure:: _static/connection_settings.png
   :name: ngmobile_ngw_connection_settings_pic
   :align: center
   :height: 10cm

   Окно ввода параметров подключения
 
6. В случае удачного подключения откроется окно с созданной учетной записью NextGIS Web.

Для подключения к NextGIS Web **вторым способом** необходимо выполнить следующую последовательность шагов:

1. Вызвать меню опций (см. :numref:`ngmobile_main_activity_pic` п. 5). 
   В меню опций необходимо выбрать пункт "Настройки" (см. :numref:`ngmobile_settings_pic`).

.. figure:: _static/settings.png
   :name: ngmobile_settings_pic
   :align: center
   :height: 10cm

   Меню опций

2. Выбрать пункт :menuselection:`NextGIS Web --> Настройки NextGIS Web` (см. :numref:`ngmobile_settings_ngw_pic`).  

.. figure:: _static/settings_NGW.png
   :name: ngmobile_settings_ngw_pic
   :align: center
   :height: 10cm
   
   Меню "Настройки"
  
3. В открывшемся меню выбрать пункт "Добавить учетную запись" (см. :numref:`ngmobile_add_entry_pic`).

.. figure:: _static/add_entry.png
   :name: ngmobile_add_entry_pic
   :align: center
   :height: 10cm

   Добавление учетной записи NextGIS Web

4. В открывшемся диалоговом окне надо ввести параметры подключения: NextGIS Web :term:`URL`,
   Имя пользователя/логин и пароль, нажать кнопку "Подключить" 
   (см. :numref:`ngmobile_ngw_connection_settings_pic`).

5. В случае удачного подключения откроется окно с созданной учетной записью NextGIS Web.

.. note::
   В диалогом окне для ввода параметров при создании подключения к NextGIS Web 
   Имя пользователя/логин и пароль вводить без пробелов!
   Mногие клавиатуры смартфонов и планшетов при автоподстановке текста, а также 
   при вставке копируемого текста из буфера обмена добавляют пробел в конце текста 
   в поле ввода (имя пользователя, пароль). Полученный текст с пробелом воспринимается 
   NextGIS Web как другое имя пользователя или другой пароль, что приводит к отказу 
   в создании подключения.


