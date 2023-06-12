# Создание своей локации "Заснеженные горы" в Unity
## Пример работы (1 часть)
![ezgif-5-b78e40db8b](https://github.com/Sazukiro/Landscape-Creating-in-Unity/assets/133951840/7190dd0d-a77f-4770-9293-b106f13fc4d2)
## О моей первой работе
Для создания данной локации мне потребовался такой объект как `"Terrain"`, который в переводе означает `"рельеф"`. С помощью него, как ни странно, я создал рельеф своей местности: горы и границы террейна из гор.

Для редактирования местности я использовал специальную кисть `"Paint Terrain"` в настройках террейна и выбрал парраметр `"Set Height"`, который позволяет рисовать возвышенности и впадины. Для создания пути или моста между двумя горами, а также для создания местности для дерева и будущей пещеры, мне пришлось установить определённую высоту возвышенности в парраметре `"Height"`, чтобы было удобно впоследствии передвигаться.

![11111](https://github.com/Sazukiro/Landscape-Creating-in-Unity/assets/133951840/fa3fd81e-a41f-4748-a017-d52ab9e5f4da)

После же я начал наносить текстуры, скачанные из [Unity Asset Store](https://assetstore.unity.com/) на уже готовый рельеф, чтобы он был более красивым. Для этого в тех же настройках пера я поменял парраметр на `"Paint Texture"`.

![2223323](https://github.com/Sazukiro/Landscape-Creating-in-Unity/assets/133951840/c50f1e66-e2c6-4056-b9e6-46cde091a37f)

---

:red_circle: **ОСТОРОЖНО**: при работе с террейном ни в коем случае не меняйте его собственную текстуру, иначе нельзя будет рисовать на нём другими текстурами.

---
Нанеся все нужные мне текстуры я приступил к созданию деревьев. Так как у меня местность "Заснеженные горы", то легко предположить, что в такой-то холодной местности деревья особо не растут, но показать весь функционал работы с террейном всё равно хочется. Поэтому я решил создать всего одно большое дерево, также скачанное из [Unity Asset Store](https://assetstore.unity.com/), для которого специально выровнял местность и покрасил её в текстуру земли.

Для создания деревьев нужно открыть следущую кисть в террейне `"Paint Trees"`, после чего добавить приобретённые [модели деревьев](https://assetstore.unity.com/packages/3d/vegetation/trees/realistic-tree-9-rainbow-tree-54622) в эту кисть (в моём случае хватит одной), установить размер кисти, количество деревьев на данную площадь и по желанию задать им высоту.

![деревья в юнити](https://github.com/Sazukiro/Landscape-Creating-in-Unity/assets/133951840/311c245f-fd5e-4afe-9bc9-002d1a26ecfe)

Далее для разнообразия локации у меня последовало создание небольшой пещеры с источником света. Пещеру я создал с помощью скачанных [моделей камней](https://assetstore.unity.com/packages/3d/props/exterior/hq-rock-pack-free-83388), из которых слепил небольшую стенку и применил ко всем компонент `"Box Collider"`, чтобы данная стенка была осязаемой. Ну, а потом используя небольшой шаблон стены, додел всю пещеру. Чтобы мой будущий персонаж мог пройти внутрь, некоторым камням я изменил коллайдер.

![пещера](https://github.com/Sazukiro/Landscape-Creating-in-Unity/assets/133951840/50eaf8c7-30a5-459f-8eed-e28c55934b57)

Источник света же я добавил через объекты и выбрал `"Point Light"`, задал свечению немного синий оттенок и настроил его диапазон.

![свет1](https://github.com/Sazukiro/Landscape-Creating-in-Unity/assets/133951840/eaf624f3-8ffe-4ff3-a450-c7a14e1b2e80) ![свет2](https://github.com/Sazukiro/Landscape-Creating-in-Unity/assets/133951840/c0af6f6d-61cb-4511-8ad5-8f3d60dcd291)

---
:large_blue_circle: **ПРИМЕЧАНИЕ**: заметил это уже после выполнения работы, для ускорения работы с пещерой или даже для более правильного её выполнения, нужно пользоваться готовыми префабами данных моделек камней, потому что они уже содержат в себе необходимые компоненты, такие как `"Box Collider"`, а также нужные текстуры.

---
   
   Также я изменил **фон(Skybox)** моей карты и добавил **тумана(fog)**, для большей атмосферы. Для этого перешёл в раздел **Window->Rendering->Lighting->Environment** и там заменил материал скайбокса на [имеющийся](https://assetstore.unity.com/packages/2d/textures-materials/sky/customizable-skybox-174576) и включил туман.

![image](https://github.com/Sazukiro/Landscape-Creating-in-Unity/assets/133951840/dd1bedbb-d057-4b2a-bed2-c29fa94a91db)![image](https://github.com/Sazukiro/Landscape-Creating-in-Unity/assets/133951840/8f2eebb8-7dc2-410a-a4d0-d064880a8fee)


Основная работа сделана. Чтобы пройтись по готовой локации и не тратить на создание и программирование игрока 1000 лет, я скачал уже [готовый ассет](https://assetstore.unity.com/packages/tools/input-management/mini-first-person-controller-174710) персонажа с некоторым мувсетом и закреплённой в нём камерой, и добавил его на мою карту.

![персонаж](https://github.com/Sazukiro/Landscape-Creating-in-Unity/assets/133951840/4cf9bbf3-d4ee-4a8d-a468-1104906dc864)
![персонаж2](https://github.com/Sazukiro/Landscape-Creating-in-Unity/assets/133951840/0be3d6c8-406e-4743-b549-ecaee157cc39)

### Ииии... готово!

![gotovo1](https://github.com/Sazukiro/Landscape-Creating-in-Unity/assets/133951840/caebca09-5f74-4244-ad66-86f7e3b418e9)
  
  
---
  
## Пример работы (2 часть)

![юнити эффекты](https://github.com/Sazukiro/Landscape-Creating-in-Unity/assets/133951840/ccf46d86-28de-45e4-b5cf-64a5ee1980f4)

## О моей второй работе
Во второй работе я добавил немного стиля:sunglasses: и рассмотрел некоторый функционал эффектов в камере.

Для начала я добавил новые компоненты эффектов в камеру персонажа (First Person Camera). Этими компонентами являются `"Post-Process Layer"` и `"Post-Process Volume"`.

- Post-Process Layer - данный компонент включает постобработку для камеры, в данном случае для `First Person Camera`, позволяет настроить сглаживание для слоя постобработки, выбрать, к какому слою будет применяться постобработка.

- Post-Process Volume - данный же компонент позволяет управлять приоритетом и смешиванием эффектов, позваляет добавлять эффекты в стек.

После добавил в "Post-Process Volume" такие эффекты как: Bloom, Vignette(Виньетка) и Color Grading.


![камера перса 3](https://github.com/Sazukiro/Landscape-Creating-in-Unity/assets/133951840/deab59e1-b4a6-4f1b-a561-75de00d362ca) ![камера перса2](https://github.com/Sazukiro/Landscape-Creating-in-Unity/assets/133951840/1d8a1d52-aa0f-4a26-9372-3e8a0c6ac547)

**Получился вот такой результат:**

![камера эффект](https://github.com/Sazukiro/Landscape-Creating-in-Unity/assets/133951840/251a3296-8917-4763-9d84-28dfe500e152)

Теперь же привяжем эффект к определённой области, например, при приближении персонажа к дереву у персонажа искажалось зрение. Для этого создадим пустой объект `"Empty"` (Game Object), после чего включим функцию `Is Trigger` в `"Box Collider"`, для того чтобы игрок мог в него проходить. Ну и в конце применим к пустому объекту знакомые нам компоненты `"Post-Process Layer"` и `"Post-Process Volume"`, и во втором компоненте добавим эффект `"Lens Distortion"` для искажения.


![image](https://github.com/Sazukiro/Landscape-Creating-in-Unity/assets/133951840/6a1c533c-6fc7-4af6-823f-947b4963d060) ![image](https://github.com/Sazukiro/Landscape-Creating-in-Unity/assets/133951840/24a0d86b-ca57-42aa-b63f-68cec5347de4)
![image](https://github.com/Sazukiro/Landscape-Creating-in-Unity/assets/133951840/9916dedf-c0c4-4a45-9694-13420cb1d4dd)




## В итоге получим нужный нам эффект при подходе к дереву:

![image](https://github.com/Sazukiro/Landscape-Creating-in-Unity/assets/133951840/498b5d35-b3cc-41ea-a5f9-42c5330264fa)

---

## Ссылка на теоретический материал:

<a href="https://www.youtube.com/watch?v=xAtoU-FnC7o&list=PLDyJYA6aTY1k_-3fFiMVoYY04jCr-QY55"><img src = "https://i.ytimg.com/vi/xAtoU-FnC7o/maxresdefault.jpg" width=80%></a>

---
