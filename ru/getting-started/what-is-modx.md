---
title: "Обзор MODX"
translation: "getting-started/what-is-modx"
---

## Что такое MODX?

MODX - это платформа приложений контента. Что это значит? Ну, это зависит от того, кто вы есть:

![](/2.x/en/getting-started/avgjoe.png)

### Конечные пользователи (средний Джо)

MODX предлагает вам систему, которая позволяет вам публиковать ваш автономный контент в Интернете в любой форме, форма или присутствие по вашему желанию. Он также предлагает полностью настраиваемый интерфейс бэкэнда, который вы можете сделать настолько простым (или сложным), сколько захотите.

Вы можете настроить все: от простого сайта до блога, полномасштабного присутствия в Интернете с помощью MODX, и сохранить свой интерфейс администратора простым и удобным в использовании. Перетащите ваши веб-страницы, чтобы изменить порядок и переместить их. Получите полный WYSIWYG просмотр ваших ресурсов. Оставьте Ресурсы неопубликованными, прежде чем закончите их. Настройте расписание ресурсов для публикации в определенное время.

MODX поможет вам организовать ваш контент так, как вы этого хотите, и получить потрясающие встроенные результаты SEO. MODX полностью совместим со 100% дружественным URL, поэтому получить mysite.com/my/own/custom/url.html невероятно просто и так же просто, как структурировать ваш сайт таким образом.

![](/2.x/en/getting-started/coolcarl.png)

### Дизайнеры (Крутой Карл)

Вы когда-нибудь хотели полной свободы с вашим HTML и CSS? Устали от взлома существующих систем, чтобы ваш дизайн работал так, как вы его компилировали? MODX не генерирует ни одной строки HTML - он оставляет дизайн интерфейса на ваше усмотрение.

Вы можете использовать MODX в качестве своей системы управления контентом (CMS), так как MODX предлагает полностью гибкие шаблоны и доставку контента без ограничений. Разместите свой CSS и изображения там, где вы хотите. И как только вы закончите проектирование, либо передайте свои обязанности по разработке вашему разработчику, либо установите дополнительные возможности прямо из менеджера. Просто.

![](/2.x/en/getting-started/badassbilly.png)

### Разработчики (Badass Billy)

Вы смотрели на разные CMS, но обнаружили, что разработка в них - либо мешанина слишком большого количества не связанных между собой сниппетов кода, либо просто недостаточно мощная или достаточно элегантная. Вы посмотрели на PHP-фреймворки и обнаружили, что у них есть все возможности, но у вас нет управления контентом и нет достаточно хорошего пользовательского интерфейса для ваших клиентов. Вам нужна мощь и гибкость инфраструктуры с пользовательским интерфейсом и управлением контентом CMS.

Ввойдите в MODX Revolution. Полностью гибкий, мощный и надежный API, построенный на принципах ООП и использующий объектно-реляционную модель на основе PDO, называемую ORM. [xPDO](extending-modx/xpdo). Добавить богатый, [Sencha](http://sencha.com) пользовательский интерфейс для ваших клиентов (полностью настраиваемый). Пользовательские свойства и наборы. Поддержка интернационализации. Встроенное распределение пакетов, так что вы можете упаковать свой код и распределить его по любой установке Revolution. Добавьте пользовательские страницы менеджера для запуска целых приложений в MODX.

## Основные понятия

MODX, по сути, имеет массу движущих частей. Основные части это:

### Ресурсы

[Ресурсы](building-sites/resources "Ресурсы") основа местоположения веб-страницы. Это может быть фактический контент HTML, или файл, ссылка для пересылки, или символическая ссылка, или что-то еще.

### Шаблоны

[Шаблоны](building-sites/elements/templates "Шаблоны") являются домом, в котором живет Ресурс. Обычно они содержат нижний колонтитул и заголовок страницы.

### Переменные шаблона (TV)

[Переменные шаблона (TV)](building-sites/elements/template-variables "Переменные шаблона (TV)") (TVs) являются настраиваемыми полями для шаблона, которые позволяют пользователю назначать динамические значения для ресурса. Отличным примером может служить TV с тегами, который позволяет указывать теги для ресурса. Вы можете иметь неограниченное количество TV на странице.

### Чанки

[Чанки](building-sites/elements/chunks "Чанки") просто небольшие блоки контента, будь то, что вы хотите внутри. Они могут содержать [Сниппеты](extending-modx/snippets "Сниппеты")или любой другой тип элемента (Сниппет, чанк, TV и т.д.).

### Сниппеты

[Сниппеты](extending-modx/snippets "Сниппеты") динамические сниппеты кода PHP, которые запускаются при загрузке страницы. Они могут делать все, что вы можете кодировать, включая создание пользовательских меню, получение пользовательских данных, тегирование элементов, обработку форм, получение твитов и т.д.

### Плагины

Плагины - это перехватчики событий, которые запускаются всякий раз, когда происходит событие. Они обычно используются для расширения ядра Revolution, чтобы что-то делать во время части процесса загрузки - например, удаление нецензурных слов в контенте, добавление словарных ссылок на слова, управление перенаправлениями для старых страниц и т.д.

### Системные настройки

Системные настройки дают вам почти бесконечные возможности конфигурации. Большинство из них установлены наилучшим образом, но некоторые вещи (такие как [дружественные urls](getting-started/friendly-urls "Использование дружественных URL")) по умолчанию отключены или могут быть улучшены для ваших конкретных потребностей, просто изменив значение параметра. После установки перейдите в «Система»> «Системные настройки» в «Менеджере» и просмотрите доступные опции. Обязательно проверьте область «Сайт» (используйте выпадающий список «Фильтровать по области ...»), там есть несколько интересных вещей для вас.

## Так что же происходит по запросу?

MODX загружает запрошенный [Ресурс](building-sites/resources "Ресурсы"), извлекает ресурсы [Шаблон](building-sites/elements/templates "Шаблоны"), а затем помещает содержимое ресурса в этот шаблон. Затем MODX анализирует итоговое объединенное содержимое, включая любые теги, которые могут быть в нем, в порядке их достижения. Оттуда он выводит ответ в браузер пользователя.

## Смотрите также

1. [Словарь терминов Revolution](getting-started/glossary)
    1. [Объяснение структуры каталогов](getting-started/directory-structure)
