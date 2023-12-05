# Mesto (версия с фронтендом и бэкендом)

Репозиторий для приложения проекта Mesto, включающий фронтенд на React.js и бэкенд на express.js

Это продолжение работы над проектом Mesto:

ссылка на репозиторий https://github.com/VladislavSerduykov/mesto-full-project

Frontend https://vladislav.student.nomoreparties.co/

Backend https://api.vladislav.student.nomoreparties.co/

Тестирование падения сервера

Для принудительного падения сервера нужно отправить `GET`-запрос на URL `/crash-test`.

После падения должна сохраняться возможность обратиться по любому другому роуту, не запуская приложение на сервере вручную.

 Структура проекта

`backend/` - бэкенд для сервера с API

`frontend/` - фронтенд на React.js

 Дополнительные возможности этой версии

- Фронтенд
  - вся функциональность приложения сохранена
- Бэкенд
  - фронтенд и бэкенд на одном сервере с доступом через домен
  - сбор логов запросов к серверу в файл `request.log`
  - сбор логов ошибок на сервере в файл `error.log`
  - доступ к серверу через ssh
  - автоматический запуск/перезапуск сервера
  - настроенный файрвол для работы с портами
  - обработка CORS-запросов на сервере
  - доступ через `https`

## Стек технологий

- сервер на `Ubuntu` в Яндекс.Облаке
- ssh-ключи для доступа к серверу
- API-сервер на `Node.js` + `express.js`
- база данных на `MongoDB` + `Mongoose`
- обновление кода на сервере через `Git`
- менеджер процессов на сервере `pm2`
- раздача фронтенда через `nginx`
- обратный прокси-сервер на `nginx`
- файрвол `ufw`
- SSL-сертификаты от `Letsencrypt`
- хранение переменных окружения в `.env`-файле
