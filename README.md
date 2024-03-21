# azattimurvaryavanyamishalyohamarkrodyavovavova
Проект уже развернут в облаке по адресу:
https://atomfinal.cry1s.ru/

## Как склонировать проект
Так как проект использует подмодули, то для клонирования проекта необходимо выполнить:

```sh
git clone https://github.com/certified-juniors/atom-final-deploy.git --recursive
```
## Как запустить проект

Для запуска проекта необходимо иметь smtp сервер с 2 ящиками:
* no-reply@example.com
* support@example.com

Чтобы запустить этот проект, выполните следующие шаги:

Скопируйте файл .env.example и переименуйте его в .env.

Откройте файл .env и настройте необходимые переменные окружения. Необходимо установить параметры smtp сервера.
Остальное можно оставить по умолчанию или изменить на свои значения.
```
# SMTP
SMTP_HOST=smtp.example.com
SMTP_PORT=2525
SMTP_NOREPLY_USERNAME=no-reply@example.com
SMTP_SUPPORT_USERNAME=support@example.com
SMTP_NOREPLY_PASSWORD=examplepass
SMTP_SUPPORT_PASSWORD=examplepass
```
Установите Docker, если вы еще этого не сделали. Вы можете скачать его с официального веб-сайта Docker.

Откройте терминал или командную строку и перейдите в директорию проекта.

Выполните следующую команду, чтобы запустить проект:
```sh
docker compose up -d --build
```
Эта команда создаст необходимые контейнеры Docker и запустит проект.

Дождитесь запуска контейнеров. Вы можете проверить журналы, чтобы отслеживать прогресс.

Вот и все! Проект теперь должен быть запущен и работать. Вы можете получить доступ к нему, используя указанные URL-адреса или порты в вашем браузере.

## Ссылки
Если вы не изменяли порты по умолчанию, вы можете получить доступ к проекту здесь:

http://localhost:3000

## Как остановить проект

Выполните следующую команду, чтобы остановить проект:
```sh
docker compose down
```
Эта команда остановит все контейнеры Docker, связанные с проектом.

Дождитесь остановки контейнеров. Вы можете проверить журналы, чтобы отслеживать прогресс.

Вот и все! Проект теперь должен быть остановлен. Вы можете закрыть терминал или командную строку.