# Microservice ToDo

## Описание

Личный менеджер задач.

Общение между микросервисами происходит с помощью gRPC.

### Аутентификация и авторизация

В качестве токена аутентификации используется JWT (пока что сервис выдает только Access Token).

JWT содержит id пользователя, логин, роли. С помощью ролей другие сервисы могут авторизовывать пользователя.

Клиенты указывают JWT в метаданных gRPC.

[![ReadMe Card](https://github-readme-stats.vercel.app/api/pin/?username=vdlald&repo=authservice)](https://github.com/vdlald/authservice)

### Доступ к базе данных

Микросервис предоставляет CRUD интерфейс для доступа к зачам и проектам пользователя. 

В качестве СУБД используется MongoDB.

[![ReadMe Card](https://github-readme-stats.vercel.app/api/pin/?username=vdlald&repo=todoservice)](https://github.com/vdlald/todoservice)

### Vaadin-клиент

Web-приложение предоставляющее доступ к основному функционалу проекта (работа с задачами, аутентификация).

[![ReadMe Card](https://github-readme-stats.vercel.app/api/pin/?username=vdlald&repo=todosclient)](https://github.com/vdlald/todosclient)
