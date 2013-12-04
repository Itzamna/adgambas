adgambas
========

Kennel of Rhodesian Ridgeback

<b>_includes</b> - папка с исполняющими заготовками

<b>_layouts</b> - папка с шаблонами

<b>en</b> - папка с английскими страницами сайта

<b>ru</b> - папка с русскими страницами сайта

<b>images</b> - папка для картинок

<b>layouts</b> - папка со стилями

index.html - главная страница сайта

Шаблоны сайта
-------

В технической части:

<b>layout: default</b> - шаблон страниц для русской версии, кроме главной

<b>layout: default_en</b> - шаблон страниц для английской версии, кроме главной

<b>layout: main</b> - шаблон главной страницы русской версии сайта

<b>layout: main_en</b> - шаблон главной страницы английской версии сайта


Includes
-------

1. Чтобы вставить фотографию, необходимо загрузить картинку в папку images и внутри страницы, где хотите разместить фото поместить такой код:

{% include photo.html link="imya-faila.jpg" height="300" %}

2. Чтобы разместить родословную собаки, в технической части страницы нужно вставить вот такой код (заменив данные на свои):

---

father: 

  name: Blomsterangens Charm By Merten
  
  titles: Ч. Интер., Ч. Финляндии, Ч. Швеции, Ч. Норвегии, Ч. Дании, HD-B, ED-0
  
father_f: 

  name: Merten
  
  titles: Ч. Интер., Ч. Франции, Ч. Швеции, Ч. Германии, Ч. VDH, Ч. Бельгии, Ч. Голландии, Ч. Люксембурга
  
father_f_f: 

  name: Vumba
  
  titles: Ч. Интер., Ч. Мира, Ч. Бельгии, Ч. Германии, Ч. Люксембурга, Ч. Нидерландов, Ч. Франции, Ч. Испании, HD-B
  
  img: vumba.jpg
  
father_f_m: 

  name: Jockular Jodi
  
father_m: 

  name: Alfalyans Betty Boop
  
father_m_f: 

  name: Ridgefaret's Charlie
  
  titles: Ч. Швеции
  
father_m_m: 

  name: Djungelkattens Adorable Ridged Alfa
  
mother:

  name: Гуми Гамба
  
  titles: Ч. России, Ч. РКФ, Ч. Молдовы, Ч. БЛР, Ч. Македонии, Ч. Клуба, Гранд Ч. России, Ч. Украины, Ю.Ч. России, T-1, ОКД-1
  
mother_f:

  name: Винсент
  
  titles: Ч. Интер, Гранд Ч. России, Ч. Клуба, Ч. РКФ, Ч. РОЛС, Ч. АНКОР, Ч. Болгарии, Ч. Молдовы, Ч. Румынии, Ч. Украины, Ч. Беларуси, Т-1, HD-A
  
mother_f_f:

  name: Саймон
  
  titles: Ч. Интер., Ч. России, Ч. Беларуси, Ч. Украины, Ч. Молдовы, Ч. Клуба, HD-A
  
mother_f_m:

  name: А'Жина
  
mother_m:

  name: Звезда Новгородская
  
mother_m_f:

  name: Rhoban Bruto
  
mother_m_m:

  name: Bassinger Tsot Exotic
  
---

В физической части страницы нужно вставить такой код:

{% include pedigree.html %}

