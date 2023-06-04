# MERN Ecommerce

## Description

Магазин электронной коммерции, созданный на основе стека MERN и использующий сторонние API.
Этот магазин электронной коммерции включает три основных различных потока или реализации:

1. Покупатели просматривают категории магазина, товары и бренды.
2. Продавцы или торговцы управляют компонентом собственного бренда.
3. Администраторы управляют и контролируют все компоненты магазина.


* функции:
   * Node предоставляет серверную среду для этого приложения.
   * Express middleware используется для обработки запросов, маршрутов
   * Схемы Mongoose для моделирования данных приложения
   * React для отображения компонентов пользовательского интерфейса
   * Redux для управления состоянием приложения
   * Промежуточное ПО Redux Thunk для обработки асинхронных избыточных действий.


## Database Seed

* Команда seed создаст пользователя-администратора в базе данных
* Электронная почта и пароль передаются команде в качестве аргументов
* Как и в приведенной ниже команде, замените скобки на адрес электронной почты и пароль.
* Для получения дополнительной информации см. код [здесь](server/utils/seed.js)

```
npm run seed:db [email-***@****.com] [пароль-******] // Это всего лишь пример.
```

## Install

Некоторые основные команды Git:
```
$ git clone 
$ cd project
$ npm install
```

## Setup

```
 Создайте файл .env, который включает:

  * MONGO_URI & JWT_SECRET
  * PORT & BASE_SERVER_URL & BASE_API_URL & BASE_CLIENT_URL
  * MAILCHIMP_KEY & MAILCHIMP_LIST_KEY => Mailchimp configuration
  * MAILGUN_KEY & MAILGUN_DOMAIN & MAILGUN_EMAIL_SENDER => Mailgun configuration
  * GOOGLE_CLIENT_ID & GOOGLE_CLIENT_SECRET & GOOGLE_CALLBACK_URL => Google Auth configuration
  * FACEBOOK_CLIENT_ID & FACEBOOK_CLIENT_SECRET & FACEBOOK_CALLBACK_URL => Facebook Auth configuration
  * AWS_ACCESS_KEY_ID & AWS_SECRET_ACCESS_KEY & AWS_REGION & AWS_BUCKET_NAME => AWS configuration
```

## Start development

```
$ npm run dev
```

## Simple build for production

```
$ npm run build
```

## Run build for production

```
$ npm start
```


## Languages & tools

- [Node](https://nodejs.org/en/)

- [Express](https://expressjs.com/)

- [Mongoose](https://mongoosejs.com/)

- [React](https://reactjs.org/)

- [Webpack](https://webpack.js.org/)


### Code Formatter

- Добавить каталог `.vscode`
- Создайте файл `settings.json` внутри `.vscode`
- Установите Prettier - средство форматирования кода в VSCode
- Добавьте следующий фрагмент: 

```json

    {
      "editor.formatOnSave": true,
      "prettier.singleQuote": true,
      "prettier.arrowParens": "avoid",
      "prettier.jsxSingleQuote": true,
      "prettier.trailingComma": "none",
      "javascript.preferences.quoteStyle": "single",
    }

```

