Охранно-пожарная сигнализация и сопряжение со смежными системами (общеобменная и противодымная приточно-вытяжная вентиляция, лифты, эскалаторы, газовое пожаротушение в серверных, водяное пожаротушение)

Проектная документация на сервере в папке `P:\Сириус Главный Медиа Центр (гп1)\Проектная документация`.

Фото, видеозаписи и исполнительные чертежи в AutoCAD-е разложены на сервере по папкам:
 - `P:\Сириус Главный Медиа Центр (гп1)\Исполнительная документация\Планы и разрезы\Этаж 1`,
 - `P:\Сириус Главный Медиа Центр (гп1)\Исполнительная документация\Планы и разрезы\Этаж 2`,
 - `P:\Сириус Главный Медиа Центр (гп1)\Исполнительная документация\Планы и разрезы\Этаж 3`,
 - `P:\Сириус Главный Медиа Центр (гп1)\Исполнительная документация\Планы и разрезы\Кровля`

![Насосная и компрессорные](https://user-images.githubusercontent.com/104857185/171544261-4c532d6e-1d3c-4a05-ba8e-2b2aca1acf58.JPG)
![7205-V2_Plan - копия](https://user-images.githubusercontent.com/104857185/171543881-4e543708-fdce-4141-bce4-7e9f0f161609.jpg)
![7205 5 4-V2_Plan](https://user-images.githubusercontent.com/104857185/171544022-b674540c-0bbd-43bc-bcbf-c25a29116c45.jpg)
![Компрессорные](https://user-images.githubusercontent.com/104857185/171544346-5e44b47b-49b2-4dbb-85ba-10ddfd316b3c.JPG)

#### Панель 16 (шлюз, GAP)
![IMG_2726](https://user-images.githubusercontent.com/104857185/171537384-c482f8e8-ee0a-4139-be72-2731192d944e.JPG)
![IMG_4644](https://user-images.githubusercontent.com/104857185/171537639-966bbdd7-f238-458b-91cf-18e4e560d9d3.JPG)
![IMG_4838](https://user-images.githubusercontent.com/104857185/171537809-222a04d8-c10b-4a70-8f21-f0596526ad6e.JPG)


#### Версия конфигуратора
![Версия конфигуратора v5](https://user-images.githubusercontent.com/104857185/171536166-94498381-1c9f-4b21-b5d8-3bd6a90bf7b4.png)

Панели и ММ-ка ведут обмен по BACNet-у. Ветки сети с панелями то одна, то другая отваливаются. В связи с этим надо внести следующие изменения:
 - переключить панели с SafedLink-а 384 кбит/сек. на локальную сеть 10 Мбит/сек. (все панели стоят в кроссовых рядом с коммутаторами локальной подсети),
 - кольцо на C-WEB с 4 панелями оставить,
 - отключить панели от SafedLink-а,
 - обновить прошивки на панелях до 50-й,
 - обновить ММ-ку 4.40 -> 4.70 (сущ. сервисный USB-вый ключ заменить),
 - перевести с BACNet-а на OPC-сервер

#### Схема сети C-WEB и SafedLink
![Схема сети C-WEB и SafedLink](https://user-images.githubusercontent.com/104857185/171536790-5f6772e3-4cc1-4c89-a544-cff10c3aa81a.jpg)

#### Адреса панелей
![Настройка сетевой платы для конфигуратора](https://user-images.githubusercontent.com/104857185/171536396-04cfb9a4-3505-46ba-a031-703e29f62c0b.png)

#### Статические маршуры между панелями и ММ-кой
![Добавление статического маршрута](https://user-images.githubusercontent.com/104857185/171542264-712bcdad-d6c3-49e7-99fc-c9a0c84540d2.png)

#### Конфигурация панелей


#### SCADA-система DMS8000 (ММ-ка)
![Версия Composer-а](https://user-images.githubusercontent.com/104857185/171541990-c5dfd4db-58a9-4f4c-8426-c8e2f8cee2c7.png)
![Версия DMS8000 с данными о Hotfix-ах](https://user-images.githubusercontent.com/104857185/171542050-9e56e80a-f688-4796-b051-77f86d28af51.png)
![Версия MM8000](https://user-images.githubusercontent.com/104857185/171542084-919d4cbc-3a68-4d4c-befd-4296c89d606e.png)

#### Настройка BACNet в компосере
![Настройки BACnet в Composer-е](https://user-images.githubusercontent.com/104857185/171542161-afc7b7ef-1e89-421a-bb9b-b8a58fd44b8a.png)
