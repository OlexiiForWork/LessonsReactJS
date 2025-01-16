# Установка и настройка среды разработки Visual Studio Code для работы с React JS

## Install Visual Studio Code
-Ссылка для скачивания Visual Studio Code : https://code.visualstudio.com/download;
## Install Node.js
- Ссылка для скачивания Node.js : https://nodejs.org/en/download;
- Команды для проверки 
 > Если `node --version` отрабатывает а другие нет то это настройки системы запрещающие выполнения скриптов на ПК. На Windows  может исправить:`Set-ExecutionPolicy Unrestricted.`

```
node --version
```
```
npx -v
```
```
npm -v
```
 - Если во время востановления зависимостей возникают проблемы, установите зависимости командой
```
npm install --legacy-peer-deps
```

## Создания проэкта ReactJS
> Команда создания проэкта ReactJS `npx create-react-app` имя проэкта(папка с проэктом) `my-app `
- Ссылка для скачивания Node.js : https://nodejs.org/en/download;
```
npx create-react-app my-app 
```
- Создания проэкта ReactJS с использованием typescript
```
npx create-react-app my-app --template typescript
```
## Visual Studio Code расшырения
- Подсветка синтаксиса
```
DotENV
```
 - Для подсвечивания типа при работе с  `TypeScript`
```
Prettify TypeScript: Better Type Previews
```
 - Описание рашерения `ES7 React`: https://marketplace.visualstudio.com/items?itemName=rodrigovallades.es7-react-js-snippets
```
ES7 React/Redux/GraphQL/React-Native snippets
```
 - Подсветка ошыбок типов
```
ESLint
```
- Подсветка изминений гита
```
GitLens
```
- Работа с CSS
```
 Tailwind CSS Intellisense
```
```
 HTML / CSS
```
```
 Toggle Quotes
```
- Добавление иконок
```
 VSCode Icons
```
- подобие Postman 
```
 RapidAPI
```

