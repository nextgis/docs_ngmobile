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

Удаление учетной записи NextGIS Web
-----------------------------------

Удаление учетной записи NextGIS Web может осуществляться несколькими способами. 
При использовании **первого способа** удаление учетной записи NextGIS Web, необходимо 
выполнить следующую последовательность шагов:

1. Вызвать меню опций (см. :numref:`ngmobile_main_activity_pic` п. 5). 
2. Далее выбрать пункт меню "Настройки" (см. :numref:`ngmobile_settings_pic`).
3. В открывшемся меню опций необходимо выбрать пункт "NextGIS Web/ Настройки 
   NextGIS Web" (см. :numref:`ngmobile_settings_ngw_pic`). 

4. В открывшемся окне необходимо выбрать ранее созданную учетную запись 
   NextGIS Web (см. :numref:`ngmobile_select_ngw_layer_pic`). 
   
5. Выбрать пункт меню "Удалить учетную запись"(см. :numref:`ngmobile_remove_account_pic`).

.. figure:: _static/remove_account.png
   :name: ngmobile_remove_account_pic
   :align: center
   :height: 10cm
    
   Удаление учетной записи NextGIS Web 

6. Удалить выбранную учетную запись NextGIS Web.
7. В случае удачного удаления откроется окно программы, в котором будет отсутствовать 
   ранее созданная учетная запись NextGIS Web.

Для удаления учетной записи NextGIS Web **вторым способом** необходимо выполнить 
следующую последовательность шагов:

1. На устройстве (мобильном телефоне/планшете) вызвать "Настройки операционной системы".
2. Перейти к Аккаунтам/Учетным записям в настройках телефона.
3. Выбрать из списка учетную запись "NextGIS Web" (см. :numref:`ngmobile_accounts_in_os_pic`).

.. figure:: _static/accounts_in_os.png
   :name: ngmobile_accounts_in_os_pic
   :align: center
   :height: 10cm
   
   Выбор в настройках ОС аккаунт NextGIS Web 

4. В открывшемся окне необходимо вырать ранее созданную учетную запись NextGIS Web,
   в нижнем правом углу экрана нажать на кнопку "Удалить уч.запись" 
   (см. :numref:`ngmobile_remove_account_in_os_pic`).

.. figure:: _static/remove_account_in_os.png
   :name: ngmobile_remove_account_in_os_pic
   :align: center
   :height: 10cm
   
   Удаление учетной записи через настройки ОС 

5. Удалить выбранную учетную запись NextGIS Web.
6. В случае удачного удаления откроется окно программы, в котором будет отсутствовать 
   ранее созданная учетная запись NextGIS Web. 

