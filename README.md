# GB_Git_Homework


# Главные возможности в Git.
## Что такое Git?
Git — распределённая система управления версиями. Проект был создан Линусом Торвальдсом для управления разработкой ядра Linux, первая версия выпущена 7 апреля 2005 года. На сегодняшний день его поддерживает Джунио Хамано. 

## Подготовка репозитория
Подготовка репозитория нужна для "активации" (инициализации) отслеживания изменений с помощью системы контроля версий (Git). Для этого нужно открыть нужную папку с данными в программе Git. После в терминале прописать команду *git init*.

## Создание "сохранений"
Создание "сохранений" (они называются коммитами) нужно для дальнейшего отслеживания и возвращения к старым версиям данных в случае необходимости. Для создания коммита нужно прописать команды *git add* и *git commit -m "info about commit"*. Также можно сократить до одной команды *git commit -a -m "info about commit"*.

## Переключение между "сохранениями"
Переход между коммитами нужен в случае какой-либо необходимости. Для этого нужно прописать команду *git checkout (first five or six characters from commit name)*

## Журнал изменений
Журнал изменений нужен для отслеживания коммитов по дате и автору в случае какой-либо необходимости. Для этого пропишите команду *git log*.

## Ветки в Git
Ветки в Git нужны для изменения данных без редактирования основной версии. Например, для ведения черновика и чистовика. Для создания ветки нужно записать команду *git branch (name branch)*.

## Слияние веток и решение конфликтов
Для переноса данных из одной ветки в другую используется слияние. Слияние производится коммандой *git merge (name incoming branch)*. При этом нужно перейти в ветку, в которую будут заноситься данные из входящей ветки по команде *git merge*.
### Также могут возникнуть конфликты при слиянии веток, если одна строка в разных ветках заполнена по разому. 
В таком случае можно выбрать один из вариантов решения:

* Accept Current Change
* Accept Incoming Change
* Accept Both Change

Есть еще возможность сравнить варианты (Compare Changes). Но это не вариант решения конфликта, а инструмент для выбора варианта решения.

## Удаление веток
При необходимости можно удалить ветку выбрав команду *git branch -d (name branch)*.

# Немного об удаленном репозитории
## Для чего он нужен.
Когда ведется разработка какого-либо ПО (программного обеспечения) не всегда разработчики находятся рядом. Из-за этого появляется необходимость быстрого взаимодействия для передачи измененных файлов. Просто передавать архивом на эл. почту очень затратно и проблематично. Для этого и появилась возможность удаленного репозитория, в который можно выгружать актуальную информацию. Например, есть сервис GitHub (github.com).

## Как выгрузить репозиторий.
Для выгрузки репозиторя нужно использовать команду *git clone (URL of distant repository).

*Примечание. Возможно, нужно будет авторизоваться на сервисе удаленного репозитория.*

## Как получить актульную версию удаленного репозитория?
Для актуализации версии локального репозитория с удаленным необходимо выполнить команду *git pull*.

## Как выгрузить последние изменения с удаленного репозитория на внешний?
Для выгрузки на локального репозитория на удаленный, используется команда *git push*.

# Возможности markdown
## Списки в markdown

Для создания списка без нумерации перед пунктом ставится * с одним отступом от информации.

Например,
* Первый ненумерованный пункт
* Второй ненумерованный пункт
* И т.д.

Для создания списка с нумерацией стасится цифра с точкой, например <1.>, и также с одним отступом от информации. 
Например,
1. Первый нумерованный пункт
2. Второй нумерованный пункт
3. И т.д.

## Разметки в markdown

* **Полужирный** или __Полужирный__

* *Курсив* или _Курсив_

* ~~Зачеркнутый~~ 

* **Полужирный и ~~_вложенный зачеркнутый курсив_~~**

* **_Все полуирным и курсивом_**

* <sub>Посдтрочный текст</sub>

* <sup>Надстрочный текст</sup>

## Цитирование
Если необходимо выделить текст как цитату другого человека, то для этого можно использовать символ ">" в начале следующей строки и после написать саму цитату.

Например, 
> Это цитата.

Это не цитата.

>Это другая цитата.

## Подставление картинки в тексте.
Для вставки картинки в тексте необходимо сначала подставить в начале строки восклицательный знак "!", потом в квадратных скобках "[]" написать суть картинки и после в круглых скобках "()" вставить ссылку на фото/путь на компьютере к фото.

Например, 
![This is an image](https://avatars.mds.yandex.net/get-zen_doc/4790423/pub_608ab9c01037af4f21d3d4ac_608abcb234055e2cb3e830a5/scale_1200)

## Добавление ссылок
Для добавление ссылки с наименованием в ней нужно само наименование информации заключить в "[]" скобки, а ссылку в "()" скобки.

Например,

>Информацию брал по ссылке на [GitHub](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#links)

## Добавление списка задач

В создании списка используют выставление меток.

Нарпимер,
- [x] Есть метка
- [ ] Нет метки
>>>>>>> daniil_koblov_gu_2906_homework
