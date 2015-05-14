# Описание #

> Плагин заменяет стандартное меню плагинов Plugin Commands. Обладает рядом расширенных возможностей: отображение дополнительной информации, упорядочивание, фильтрация при наборе, возможность сокрытия ненужных или редко используемых команд.

> По умолчанию диалог показывает только те плагины, которые доступны в текущем контексте (панель файлов, редактор и т.д). По нажатию клавиш Ctrl-H будет показан полный список плагинов. Те из них, которые недоступны в текущем контексте отмечены точкой спереди. Их команды вызывать нельзя.

> Все возможности по отображению расширенной информации включаются непосредственно в диалоге, через горячие клавиши (их описание - в справке). Для начала фильтрации набирайте текст, удерживая кнопку Alt. По умолчанию, вводимый текст ищется по началу каждого слова. Для фильтрации по вхождению набирайте первым символом "".

> Для Far 2/3 поддерживается возможность динамической выгрузки и загрузки плагинов, аналогичная командам "unloadp:" и "pload:". Плагины выгружаются по команде "Del". Чтобы загрузить плагин обратно, включите режим показа недоступных плагинов (Ctrl-H), выгруженные плагины помечаются "X". Команда загрузки плагина - "Ins".

> Обсуждение: http://forum.farmanager.com/viewtopic.php?f=5&t=3608

## Загрузить ##

  * [Последняя версия](http://plugring.farmanager.com/plugin.php?pid=882)

  * [Старые версии](http://code.google.com/p/far-plugins/downloads/list?q=PlugMenu&can=1)



---


# История изменений #

## Ver 1.21 ##

  * Переход на страницу плагина на Plugring (Ctrl-PgUp в списке плагинов или кнопка Plugring в диалоге информации о плагине)

  * Исправлено несколько ошибок

## Ver 1.20 ##

  * Far3 build 2927+

  * Вывод столбцов Автор (Ctrl6) и Версия (Ctrl7). Только для Far3

  * Добавлены заголовки столбцов. Клик на заголовке упорядочивает по столбцу, правый клик - меню упорядочивания. Заголовки можно отключить в настройках.

  * По F2 (или по правому клику на плагин) открывается меню команд.

  * По F3 выдается более полная информация о плагине (для Far3)

  * В версии для Far3 снова отслеживается время вызова плагина

  * Исправлено несколько ошибок


## Ver 1.0.16 ##

  * Far3 build 2415+

## Ver 1.0.15 ##

  * Возможность переименования команд (F4). Только в версии для Far 3.

  * Расширенные опции сортировки (Ctrl-F12)


## Ver 1.0.14 ##

  * Поддержка Far3 (см. Описание)


## Ver 1.0.13 ##

  * Поддержка большого экранного буфера. Требуется Far 2 build 1573+


## Ver 1.0.12 ##

  * Исправлена ошибка с показом ансишных плагинов в Far/2

  * Добавлен английский хелп by farman.


## Ver 1.0.11 ##

  * Для работы юникодной версии плагина требуется Far/2 build 1148+

  * Поддерживается ключ /p с указанием нескольких путей

  * Исправлена ошибка со слетом 64-х разрядной версии


## Ver 1.0.10 ##

  * Для Far/2: Добавлены префиксы командной строки "PlugLoad:" и "PlugUnload:"

> Данные команды являются полными аналогами команд PLoad и Unloadp стандартного плагина FAR Commands. За тем исключением, что плагин PlugMenu не "видит" плагины, загруженные "в обход" него и не может правильно отобразить их команды. Так что, предпочтительнее использовать его команды.

  * Так же новые плагины можно подключать из списка команд, через диалог "Load Plugin", вызываемый по Ctrl-L.

  * Префикс PlugMenu: может иметь необязательный параметр - маску для фильтрации списка команд


## Ver 1.0.9 ##

  * Добавлена поддержка персональных плагинов (диалог "System settings", опция "Path for personal plugins")

  * Добавлено меню опций. Вызывается по команде F2.

  * Опции: "Следить за мышью" и "Циклическая прокрутка"

  * Исправлено несколько ошибок


## Ver 1.0.8 ##

  * Изменен алгоритм сканирования кэша плагинов.

  * Для работы юникодной версии плагина требуется Far/2 build 910+


## Ver 1.0.7 ##

  * Плагины, вызываемые из PlugMenu теперь должны нормально показывать прогресс-индикаторы и прочие окна состояния

  * Для Far/2: метки ансишных плагинов теперь показываются отдельным столбцом. Их можно опциноально прятать по команде Ctrl+Shift+1.

  * Для работы юникодной версии плагина требуется Far/2 build 853+


## Ver 1.0.6 ##

  * Исправлена ошибка с показом многострочных ансишных плагинов в Far/2

  * Хоткеи в меню плагинов теперь должны быть независимы от раскладки клавиатуры. Чтобы это работало, в фаре должно быть настроено XLAT преобразование.


## Ver 1.0.5 ##

  * Окно PlugMenu теперь использует custom control - grid.

  * Возможна фильтрация по любому столбцу (имени DLL, флагам и датам).

  * Подсвечивается часть строки, совпадающая с фильтром.

  * Скрытые и недоступные плагины теперь отмечаются цветом, все цвета настраиваются через файл Settings.reg

  * Немного изменены хоткеи:

> Ctrl+H        - Включает/выключает показ недоступных и скрытых плагинов

> Ctrl+Shift+H  - То же, только для скрытых плагинов.

  * Интеграция с FarHints (требуется FarHints ver 1.0.14+)

  * Исправлено несколько ошибок


## Ver 1.0.4 ##

  * Добавлена поддержка ключа Far /u (именные настройки)

  * Добавлен диалог "Информация о плагине" (вызывается по нажатию F3)

  * Исправлено несколько ошибок


## Ver 1.0.3 ##

  * В режиме сортировки по-умолчанию все недоступные в текущем контексте плагины располагаются в конце списка. Включение режима - Ctrl-F11

  * Меню выбора режимов сортировки (для забывчивых) - Сtrl-F12

  * Только в версии для Far 2: поддержана возможность выгрузки/загрузки плагинов "на лету", аналогичная командам "unloadp:" и "pload:"

> Плагин выгружается по нажатию "Ctrl-Del". Выгруженные плагины видны в списке, если включен режим показа недоступных плагинов, они помечены символом "x". Загрузить его обратно можно по нажатию "Ins".

> Однако, если выгружать плагин по команде "uloadp:", то PlugMenu это не видит, и показывает плагин в списке доступных, хотя его команды вызвать не может. Как это исправить - пока не знаю.

  * Юникодная версия требует Far 2 build 680


## Ver 1.0.2 ##

  * Добавлена возможность скрывать из списка команд редко используемые или ненужные плагины. Это делается через диалог настройки, вызываемый по F4.

> Обратите внимание, что плагины скрываются только из расширенного меню, в стандартном меню они остаются видимыми, соответственно эта настройка не влияет на макросы, работающие через F11.

> Нажатие Ctrl-H по очереди включает показ сначала скрытых, а потом недоступных в текущем контексте плагинов. Скрытые/недоступные плагины помечаются разными значками в меню.


## Ver 1.0.1 ##

  * Добавлена поддержка плагинов, добавляющих несколько строк в меню

  * Режим фильтрации в меню плагинов можно включить/выключить нажатием Alt

  * Улучшена совместимость с менеджером плагинов Underscore

  * Версия для Far 1.8