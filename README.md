##Передача файлов без сохранения на сервере.

1. **Приложение использует node.js(express, socket.io) на сервере и HTML5 File API на клиенте.**

  Сервер `node app.js`

  Страница отправки файла: `http://localhost:8080/`

  Страница получения файла: `http://localhost:8080/receiver`

  Отправитель выбирает файл и подтверждает выбор. На странице появляется индикация отправки. Такая же индикация присутствуети на странице получения файла. После того как обмен данными успешно завершен - на странице получения появляется ссылка для загрузки файла.

  *Протестировано в последних версиях Firefox и Chrome.*


2. **Обмен данными с помощью WebRTC Data Channel**

  WebRTC позволяют обмениваться данными между браузерами в режиме реального времени. На данный момент доступны в Firefox Beta/Aurora и Chrome Canary. 

  *Работа WebRTC Data Channel (rtc_data.html) протестирована в Firefox 21 Aurora.*
