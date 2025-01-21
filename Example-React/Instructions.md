# Инструкцыя: Создание React JS приложения и первий запуск

## Создание React JS. Сперва желательно выполнить шаги по установке Node.js смотрите README.md урок 1.
### React JS
 > Создание приложения React JS имя проэкта(директория) `example-react-js`
 
 > [!WARNING]
 > Если возникают ошыбки во время установки зависимостей, выполните команду `npm config set legacy-peer-deps true` и пересоздайте проэкт
```
 npx create-react-app example-react-js;
```
### старт проэкта

 > [!WARNING]
 > Если возникают ошыбки во время старта, что не найдены какието пакеты установите их пример: `npm install ajv@latest ajv-keywords@latest`
```
cd example-react-js
npm start
```

---

В папке `example-react-js` 3 папки и 3 файла.  `node_modules` это папка куда устанавливаються все дополнительные пакеты.
Дополнительная папка `public` эта папка содержыт подолнительнные файлы ресурсов, картинки и другие.
Основная папка с проэктом `src` эта папка содержыт нашь код.
Файлы с описанием проэкта: `package-lock.json, package.json`.
```
d----- node_modules
d----- public
d----- src
-a----  package-lock.json
-a----  package.json
-a----  README.md
```
Содержымое `src` с коментариями. Удалим с проэкта лишние файлы.
```
-a---- App.css               --- Стили для файла App.js.
-a---- App.js                --- Файл с основнным компонентом.
-a---- App.test.js           --- (Файлы для удаления)
-a---- index.css             --- Стили для файла index.js.
-a---- index.js              --- Основной файл проэекта,  точка входа.
-a---- logo.svg
-a---- reportWebVitals.js    --- (Файлы для удаления)
-a---- setupTests.js         --- (Файлы для удаления)
```
