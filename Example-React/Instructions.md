# Инструкцыя: Создание React JS приложения и первий запуск

## Создание React JS. Сперва желательно выполнить шаги по установке Node.js смотрите README.md урок 1.
### React JS
 > Создание приложения React JS имя проэкта(директория) `example-react-js`.
   > Первое приложение [React JS](https://ru.legacy.reactjs.org/docs/create-a-new-react-app.html)
 
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

С файла `index.js` удалим строки.
```TypeScript
import reportWebVitals from './reportWebVitals';
```
```TypeScript
reportWebVitals();
```

 Изменим содержымое файла `App.js` изменим содержымое на 
 - https://ru.legacy.reactjs.org/docs/refs-and-the-dom.html.
 - https://ru.legacy.reactjs.org/docs/context.html.

```TypeScript
import React from 'react';
//import logo from './logo.svg';
import './App.css';

class App extends React.Component {
  constructor(props) {
    super(props);

    this.textInput = null;

    this.setTextInputRef = element => {
      this.textInput = element;
    };

    this.focusTextInput = () => {
      // Устанавливаем фокус на текстовом поле ввода с помощью чистого DOM API
      if (this.textInput) this.textInput.focus();
    };
  }

  componentDidMount() {
    // устанавливаем фокус на input при монтировании
    this.focusTextInput();
  }

  render() {
    // Используем колбэк в `ref`, чтобы сохранить ссылку на DOM-элемент
    // поля текстового ввода в поле экземпляра (например, this.textInput).
    return (
      <div>
        <input
          type="text"
          ref={this.setTextInputRef}
        />
        <input
          type="button"
          value="Focus the text input"
          onClick={this.focusTextInput}
        />
      </div>
    );
  }
}

export default App;
```

React вызовет ref колбэк с DOM-элементом при монтировании компонента, а также вызовет его со значением null при размонтировании. Рефы будут хранить актуальное значение перед вызовом методов componentDidMount или componentDidUpdate.

стартуем приложение
```npm
npm start
```

Проведите измин по эксперементируйте
