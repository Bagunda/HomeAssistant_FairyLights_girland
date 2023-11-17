# HomeAssistant_FairyLights_girland
Управление светодиодной гирляндой Fairy Lights Model MSL9 (Tuya) через интеграцию для локального (безоблачного) управления гирляндой.

По уроку от Kvazis https://www.youtube.com/watch?v=WGPL-l1oZIs сделана доработка программы и интерфейса. Всю суть смотри там.

![image](https://github.com/Bagunda/HomeAssistant_FairyLights_girland/assets/16766521/ce15adf0-e950-4508-9909-2ad694c64703)

Добавлено управление яркостью когда мигает сцена.
Добавлен интерфейс (страничка, панель), на которой выведены сущности как на видеоролике. И добавлено 20 кнопок для быстрого включения одной из 20 сцен.

Код [da_fairy_lights.yaml](https://github.com/Bagunda/HomeAssistant_FairyLights_girland/blob/main/packages/da_fairy_lights.yaml) у меня добавлен в папку `/includes/packages/da_fairy_lights.yaml` через пакаджи.
Для этого в `configuration.yaml` надо чтобы была включена вот такие строчки:
```
homeassistant:
    packages: !include_dir_merge_named includes/packages/
```

Если у вас интерфейс не работает, то читайте ошибку и добавляйте отсутствующие элементы.
Например: [mushroom-card](https://github.com/piitaya/lovelace-mushroom).

Чтобы добавить карточки на панель (чтобы был такой же интерфейс) - добавтье новую панель.
Справа сверху нажмите три точки и выберите "Изменить панель"

![image](https://github.com/Bagunda/HomeAssistant_FairyLights_girland/assets/16766521/f8b29bb9-3dfe-48f5-b392-315f970ff7c2)

Справа сверху нажмите три точки и выберите "Текстровый редактор"

![image](https://github.com/Bagunda/HomeAssistant_FairyLights_girland/assets/16766521/a7cf8e8e-f8e3-410c-8b63-ef1e5d4beb58)

И вставьте туда код из моего файла [lovelace.yaml](https://github.com/Bagunda/HomeAssistant_FairyLights_girland/blob/main/lovelace.yaml)

![image](https://github.com/Bagunda/HomeAssistant_FairyLights_girland/assets/16766521/897f70b0-e66f-4c2d-9e66-7c470bc516c8)

И поменяйте в обоих местах имена сущностей с моих на те что у вас получились.
