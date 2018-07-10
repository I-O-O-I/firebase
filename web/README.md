# Firebase Web Codelab - Start code

This folder contains the starting code for the [Firebase: Build a Real Time Web Chat App Codelab](https://codelabs.developers.google.com/codelabs/firebase-web/).

If you'd like to jump directly to the end and see the finished code head to the [web](../web) directory.

## Чтобы запустить проект необходимо

Чтобы установить или обновить CLI, выполните следующую команду npm:
`npm -g install firebase-tools`

Чтобы убедиться, что CLI установлен правильно, откройте консоль и запустите:
`firebase --version`

Убедитесь, что версия Firebase CLI выше 3.5.0, так что у нее есть все последние функции, необходимые для облачных функций. Если нет, выполните npm install -g firebase-toolsобновление, как показано выше.

Авторизовать CLI Firebase, выполнив:
`firebase login`

Убедитесь, что вы находитесь в папке web, затем настройте CLI Firebase, чтобы использовать проект Firebase:
`firebase use --add`

При использовании Firebase SDK для облачных функций ваш код функций будет находиться в functionsкаталоге (по умолчанию). Код ваших функций также является приложением Node.js и поэтому нуждается в package.jsonтом, чтобы предоставить некоторую информацию о ваших приложениях и списках зависимостей.

В файле package.json уже указаны две требуемые зависимости: Firebase SDK для облачных функций и SDK Firebase Admin . Чтобы установить их локально npm installиз functionsпапки:
`cd functions && npm i`
`cd ../ && firebase deploy --except functions`

Для более подробной информации [CodeLab](https://codelabs.developers.google.com/codelabs/firebase-cloud-functions/#0)
