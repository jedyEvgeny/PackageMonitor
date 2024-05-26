<h2 align="center">Трекер посылок</h2>
<h3 align="center">    
    <img src="https://img.shields.io/badge/go-%2300ADD8.svg?style=for-the-badge&logo=go&logoColor=white">
    <img src="https://img.shields.io/badge/sqlite-%2307405e.svg?style=for-the-badge&logo=sqlite&logoColor=white">
    <img src="https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black">
    <img src="https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white">
    <img src="https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white">
    <img src="https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white">
    <img src="https://img.shields.io/badge/github%20actions-%232671E5.svg?style=for-the-badge&logo=githubactions&logoColor=white">
    <img src="https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white">
</h3>


<h3>1. Описание </h3>

Сервис отслеживания посылок: регистрация посылки, получение списка посылок конкретного человека, изменение статуса посылки и т.д. Предусмотрено автоматическое тестирование и публикация приложения в DockerHub.
Стек: Go, SQLite, Docker, Git, Linux, REST API, CI/CD, Postman, DB Browser, стандартные и внешние библиотеки Go, тестирование с пакетом testify.
![Фронтенд ПО](https://github.com/jedyEvgeny/YPGoFinalJob/assets/97782789/64f3996a-914b-400c-b55d-2a8c15749cef)


<h3>2. Особенности</h3>


   
API содержит следующие операции:
- добавить задачу;
- получить список задач;
- удалить задачу;
- получить параметры задачи;
- изменить параметры задачи;
- отметить задачу как выполненную.

Ниже иллюстрация интерфейса добавления новой задачи.
![Интерфейс задачи](https://github.com/jedyEvgeny/YPGoFinalJob/assets/97782789/a7a07180-16f9-4941-9061-ad50a623c4bf)


<h3>3. Особые сведения</h3>
   
- В директории `tests` находятся тесты для проверки реализованного API. Тесты написаны сторонним разработчиком.
- Директория `web` содержит файлы фронтенда. Фронтенд написан сторонним разработчиком.

<h3>4. Запуск приложения</h3>
   
- Склонируйте приложение на локальный компьютер;
- Запустите приложение из терминала командой `go run main.go`
- Перейдите в браузере на `http://localhost:7540/`

![Пример работы приложения](https://github.com/jedyEvgeny/YPGoFinalJob/assets/97782789/9baad391-b2f1-42e9-ae11-ce24fb054c20)



<h3>5. ЛИЦЕНЗИЯ</h3>

Этот проект лицензирован согласно условиям лицензии MIT. См. файл [LICENSE](https://github.com/jedyEvgeny/YPGoFinalJob/blob/main/LICENSE) для получения дополнительной информации.
