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

<h3>2. Особенности</h3>

Фронтенда нет - работа с сервисом только через терминал.
Информация о посылках хранится в БД. Посылка может быть зарегистрирована, отправлена или доставлена. При регистрации посылки создаётся новая запись в БД. Только что зарегистрированной посылке присваивается статус «зарегистрирована». 
Трек-номер посылки равен её идентификатору в БД. Если посылка в статусе «зарегистрирована», можно изменить адрес доставки или удалить посылку.
1.1. Написано приложение.
1.2. Написаны интеграционные тесты с подключением к БД для проверки краевых случаев работы приложения.
1.3. Создан и настроен Dockerfile.
1.4. Создан и настроен workflow для автоматического тестирования и публикации приложения в DockerHub. 
   ![Вывод в терминал](https://github.com/jedyEvgeny/YP12SprintPractice/assets/97782789/ffd5119b-afe8-49af-9a33-eebab18f186b)


<h3>3. Особые сведения</h3>

Структура ParcelService реализует логику работы с посылками и использует объект типа ParcelStore для работы с данными о посылке в БД.
В качестве СУБД используется SQLite. Файл с БД называется tracker.db. В БД одна таблица parcel со следующими колонками:
`number` — номер посылки, целое число, автоинкрементное поле.
`client` — идентификатор клиента, целое число.
`status` — статус посылки, строка.
`address` — адрес посылки, строка.
`created_at` — дата и время создания посылки, строка.

<h3>4. Запуск приложения</h3>
   
- Склонируйте приложение на локальный компьютер;
- Запустите приложение из терминала командой `go run main.go parcel.go`


<h3>5. ЛИЦЕНЗИЯ</h3>

Этот проект лицензирован согласно условиям лицензии MIT. См. файл [LICENSE](https://github.com/jedyEvgeny/YP12SprintPractice/blob/main/LICENSE) для получения дополнительной информации.
