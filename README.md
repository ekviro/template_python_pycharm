## Пустой проект для начала работы на питоне в pycharm

### Установка языка программирования python
Установить python (язык + интерпретатор).

Для Windows: При установке отметить флаг "Add Python to PATH" (Добавить Python в переменную среды Path). Это позволит запускать питон из любой папки при необходимости.

https://www.python.org/?hl=RU

### Установка PyCharm Community Edition
Скачать бесплатную версию Community Edition (не Professional) и установить.

https://www.jetbrains.com/pycharm/

### Скопировать ссылку на репозиторий
![image](https://github.com/ekviro/template_python_pycharm/assets/46021781/0b46512f-9507-491c-972e-e99951e7340e)

### Создать новый проект в PyCharm - клон репозитория
Запустить PyCharm (все другие проекты закрыть).

![image](https://github.com/ekviro/template_python_pycharm/assets/46021781/f4f21e98-fad4-4b12-ab51-071d80a3fb7a)

![image](https://github.com/ekviro/template_python_pycharm/assets/46021781/ce492304-ecd3-4fee-92f2-59d1e9cdb2d2)

![image](https://github.com/ekviro/template_python_pycharm/assets/46021781/49895ce7-265e-400c-8792-99ccd36fe4d5)


Обязательно нужно создать виртуальное окружение venv в папке проекта, куда установятся зависимости (библиотеки) из requirements.txt и указанная версия интерпретатора python. Если все выполнено правильно, то по умолчанию все поля уже будут заполнены примерно как на рисунке (название виртуального окружения venv лучше не менять, так как оно уже учтено как дефолтное в .gitignore).

![image](https://github.com/ekviro/template_python_pycharm/assets/46021781/510b03ab-3e13-4c66-93b2-3580e9824c58)

После нажатия на кнопку ОК начнется установка библиотек из файла requirements.txt и выбранного интерпретатора python (процесс установки отобразится в нижней строке программы).

### Проверка успешной установки и настройки проекта
Корректность установки библиотек можно посмотреть в свойствах проекта.

![image](https://github.com/ekviro/template_python_pycharm/assets/46021781/1a37e511-632d-4d23-9ed1-494b5ff44346)

![image](https://github.com/ekviro/template_python_pycharm/assets/46021781/0adbe855-c96a-4373-9337-bb9ca77edacb)

В проводнике Windows папка с проектом будет выглядеть так:

![image](https://github.com/ekviro/template_python_pycharm/assets/46021781/45e35ae4-7cbc-4882-aebb-8df2367b6a84)














