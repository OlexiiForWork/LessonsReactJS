Инструкцыя: Создание React JS приложения и первий запуск 

## Создание React JS. Сперва желательно выполнить шаги по установке Node.js смотрите README.md
- [Metanit] https://metanit.com/web/react/;
- [ReactJS] https://react.dev/learn/start-a-new-react-project;
- [YouTube] React TypeScript ПОЛНЫЙ КУРС 2021. Props, Events, Router, Hooks, Requests.: https://www.youtube.com/watch?v=92qcfeWxtnY
- Инструуция по подготовке к работе:https://pnn.com.ua/blog/detail/how-to-install-node-js-and-npm-on-windows-and-mac
### React JS
 > Создание приложения React JS имя проэкта(директория) `example-react-js`
 
 > [!WARNING]
 > Если возникают ошыбки во время установки зависимостей, выполните команду `npm config set legacy-peer-deps true` и пересоздайте проэкт
```
 npx create-react-app example-react-js;
```
 > Создание приложения React JS с использованием `TypeScript` имя проэкта(директория) `example-react-js-typescript`
```
 npx create-react-app example-react-js-typescript --template typescript
```
### старт проэкта
```
cd <папка>
```

 > [!WARNING]
 > Если возникают ошыбки во время старта, что не найдены какието пакеты установите их пример: `npm install ajv@latest ajv-keywords@latest`
```
npm start
```

