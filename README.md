# Пустой проект для начала работы на питоне в pycharm (шаблон)


## Установка языка программирования python
Установить python (язык + интерпретатор + стандартные инструменты). В него уже входит venv (инструмент для создания виртуального окружения) и pip (менеджер пакетов Python для установки библиотек).

**Для Windows:** При установке отметить флаг "Add Python to PATH" (Добавить Python в переменную среды Path). Это позволит запускать питон из любой папки при необходимости.

https://www.python.org/?hl=RU

## Проверка установки pip и venv
**Для Windows.**

### Проверить, установлен ли уже pip, командой в cmd:
```
pip --version
```

или:
```
pip -V
```

### Если версия pip старая, то можно обновить командой в cmd:
```
python -m pip install -U pip
```

### Проверить, что установлена виртуальная среда venv:
```
python -m venv --help
```
Если ок, то появится справка.

_Примечание: venv - не тоже самое, что virtualenv. Venv более современный и устанавливается вместе с питоном. Virtualenv - более старый и его надо устанавливать отдельно (после создания старой виртуальной среды в проекте обычно там есть папка bin, а в новой venv  - нет bin)._

## Установка PyCharm Community Edition
Скачать бесплатную версию Community Edition (не Professional) и установить.

https://www.jetbrains.com/pycharm/

## Скопировать ссылку на репозиторий
<img src="https://github.com/ekviro/template_python_pycharm/assets/46021781/0b46512f-9507-491c-972e-e99951e7340e" width="700">

## Создать новый проект в PyCharm - клон репозитория
Запустить PyCharm (все другие проекты закрыть).

> **ВАЖНО:** на этом этапе или при переносе проекта в другой репозиторий нужно будет авторизоваться на github в PyCharm (следовать инструкциям внутри программы, обычно авторизация проиходит через перенаправление на страницу сайта в браузере).

<img src="https://github.com/ekviro/template_python_pycharm/assets/46021781/f4f21e98-fad4-4b12-ab51-071d80a3fb7a" width="700">

<img src="https://github.com/ekviro/template_python_pycharm/assets/46021781/ce492304-ecd3-4fee-92f2-59d1e9cdb2d2" width="700">

<img src="https://github.com/ekviro/template_python_pycharm/assets/46021781/49895ce7-265e-400c-8792-99ccd36fe4d5" width="700">


Обязательно нужно создать **виртуальное окружение venv** в папке проекта, куда установятся зависимости (библиотеки) из `requirements.txt` и указанная версия интерпретатора python. Если все выполнено правильно, то по умолчанию все поля уже будут заполнены примерно как на рисунке (название виртуального окружения **venv** лучше не менять, так как оно уже учтено как дефолтное в .gitignore).

<img src="https://github.com/ekviro/template_python_pycharm/assets/46021781/510b03ab-3e13-4c66-93b2-3580e9824c58" width="700">

После нажатия на кнопку ОК начнется установка библиотек из файла `requirements.txt` и выбранного интерпретатора python (процесс установки отобразится в нижней строке программы).

## Проверка успешной установки и настройки проекта
Корректность установки библиотек можно посмотреть в свойствах проекта.

<img src="https://github.com/ekviro/template_python_pycharm/assets/46021781/1a37e511-632d-4d23-9ed1-494b5ff44346" width="700">

<img src="https://github.com/ekviro/template_python_pycharm/assets/46021781/0adbe855-c96a-4373-9337-bb9ca77edacb" width="700">
  
В проводнике Windows папка с проектом будет выглядеть так:

<img src="https://github.com/ekviro/template_python_pycharm/assets/46021781/9efa785b-48a7-4b7a-a316-964f9f7eec54" width="700">

## Перенос проекта в новый репозиторий на github (ОБЯЗАТЕЛЬНЫЙ ШАГ)
Выбрать в меню публикацию проекта в **новый репозиторий github** (чтобы не сохранять изменения в шаблонный проект).

<img src="https://github.com/ekviro/template_python_pycharm/assets/46021781/a23601f4-7538-4f43-a30c-3f6c79bb3d59" width="700">

В предупреждении будет указано, что проект уже опубликован, но нажимаем **"Все равно опубликовать"**.

<img src="https://github.com/ekviro/template_python_pycharm/assets/46021781/190f6432-65ee-469e-9634-e61493976154" width="700">

Нужно залогиниться на github.

<img src="https://github.com/ekviro/template_python_pycharm/assets/46021781/954bcd7d-9bd6-44a7-bc47-a6b2de0d8122" width="700">

В открывшемся браузере нажать кнопку авторизации. Если в браузере не сохранены логин и пароль для github, то ввести их вручную.

<img src="https://github.com/ekviro/template_python_pycharm/assets/46021781/382082c0-06e0-4866-aa7f-c1ce45242b80" width="700">

В случае успеха появится надпись.

<img src="https://github.com/ekviro/template_python_pycharm/assets/46021781/d8e2d612-08ba-4ca8-b1d7-7fff1d873b96" width="700">

После этого можно вернуться к проекту в PyCharm.

<img src="https://github.com/ekviro/template_python_pycharm/assets/46021781/c92c7939-9ad5-485a-9456-8a34c9087c04" width="700">

Имя проекта и расположение на локальном диске останется прежним, а на github будет создан новый репозиторий с заданным именем. Теперь проект привязан к новому репозиторию.

<img src="https://github.com/ekviro/template_python_pycharm/assets/46021781/8c55363e-f726-4bfa-a39a-fc2ecfaba214" width="700">

## Как в локальном проекте установить новые библиотеки и обновить файл requirements.txt с зависимостями
В свойствах проекта нажать +

<img src="https://github.com/ekviro/template_python_pycharm/assets/46021781/4fe6e6af-f3cc-47e7-9a5c-c1adf64891b9" width="700">

Найти и установить нужную библиотеку (если поиск сразу не сработал, нажать кнопку с обновлением списка). Например, для работы с таблицами Excel

<img src="https://github.com/ekviro/template_python_pycharm/assets/46021781/7091937f-e4c2-4a51-bdf4-05e7e0e64f14" width="700">

После установки всех необходимых библиотек нужно закрыть окно свойств проекта и открыть терминал (значок внизу или найти пункт в меню).

<img src="https://github.com/ekviro/template_python_pycharm/assets/46021781/bedd1b94-3011-4625-a741-4dc0d2b23f8b" width="700">

В скобках перед путем к проекту должно быть название виртуального окружения. Тогда список зависимостей будет корректно выгружен для текущего проекта.

> (venv) C:\project_1>

Выполнить команду:
```
pip freeze > requirements.txt
```
Файл перепишется с учетом актуальных библиотек. Далее его можно будет закоммитить в репозиторий.

<img src="https://github.com/ekviro/template_python_pycharm/assets/46021781/92269424-b4a4-43bc-908c-8b600c990d44" width="700">























