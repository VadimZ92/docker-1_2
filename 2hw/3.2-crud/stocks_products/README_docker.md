Клонируем репозиторий
Переходим в папку с репозиторием: "cd \docker\2hw\3.2-crud"
Создаем образ: "docker build . --tag=[имя образа]"
Создаем контейнер: "docker run -d -p 7880:7447 --name=container_my_[имя контейнера] [имя образа]"
    порт 7880 можно выбрать любой, порт 7447 - задан в dockerfile
С помощью Visual Studio Code открываем файл requests-examples.http, в строке @baseUrl = http://localhost:7880
    ставим свой выбранный порт, сохраняем.
Проводим POST и GET запросы.