# Transactions Manager

Project designed to validate a simple application for transactions between users.
The basic proposal followed the following flow:
- Create a transaction
- Check the transaction lists
- View the total balance resulting from the transactions.

However, this flow generates some questions about security and architecture of the app:
- Who can create a transaction?
- Whose transaction for which?
- Can other users see my transactions or balance?
- How to validate a user?

Considering these points raised, the app was made to answer these problems, conserving the initial scope of transactions between users. Thus creating the need for a user to create his user with identification and password, adding an architectural and security layer.
Now the app follows the following flow:
- User creates or logs in with his account
- See your transactions sent or received.
- Creates a transaction (Validates password, balance and if the other user exists in the bank).

Note: Since there is no api available, the entire flow was done offline using the realm database, it is possible to create more than one user in the same app, and these users make transactions with each other using the same app, with the transactions being shown after the user logs in.

## 📷 Screenshots

<div style="display:flex;" >
  <img style="margin-left:10px;" src="https://i.ibb.co/Nyq93Pn/Screen-Shot-2020-08-17-at-09-53-26.png" width="19%" >
  <img style="margin-left:10px;" src="https://i.ibb.co/fdrdw1V/Screen-Shot-2020-08-17-at-09-53-35.png" width="19%" >
  <img style="margin-left:10px;" src="https://i.ibb.co/qyfwz3k/Screen-Shot-2020-08-17-at-09-53-51.png" width="19%" >
  <img style="margin-left:10px;" src="https://i.ibb.co/5Kv63SJ/Screen-Shot-2020-08-17-at-09-55-57.png" width="19%" >
  <img style="margin-left:10px;" src="https://i.ibb.co/Pxdg8m4/Screen-Shot-2020-08-17-at-09-56-04.png" width="19%" >
</div>
<div style="display:flex; margin-top:10px margin-bottom:10px" >
  <img style="margin-left:10px;" src="https://i.ibb.co/YN01VFY/Screen-Shot-2020-08-17-at-09-56-20.png" width="19%" >
  <img style="margin-left:10px;" src="https://i.ibb.co/JtKKjsJ/Screen-Shot-2020-08-17-at-09-56-32.png" width="19%" >
  <img style="margin-left:10px;" src="https://i.ibb.co/Qvryx5J/Screen-Shot-2020-08-17-at-09-57-05.png" width="19%" >
</div>
<br />

## 📦 Getting started

Installing Dependencies:

```sh
$ yarn
```

Running the app:

```sh
$ yarn start
```

For starting the app on a specfic OS:

```sh
$ yarn ios | yarn android
```

To run on ios devices you need to run the code first

```
$ npx pod-install
```

<br />

## 👩🏾‍💻 Development

- Eslint is used in the project to enforce code style and should be configured in your [editor](https://eslint.org/docs/user-guide/integrations).

- Typescript is used in the project for typechecking and should be configured in your [editor](https://github.com/Microsoft/TypeScript/wiki/TypeScript-Editor-Support).

You can also check this manually by running:

```sh
$ yarn lint
```

<br />

## 🛠 Testing

Use the following command to run unit tests with coverage:

```
$ yarn test --coverage
```

Use the following to update unit tests

```
$ yarn test -u
```

Use the following to run unit tests in watch mode while developing:

```
$ yarn test --watch
```

<br />

## 📁 Folder Structure

```
src
├── assets
│
├── components
│     └── Component (DRY)
│           ├── index.tsx
│           └── styles.tsx
├── contexts
│      └── React Context
│
├── helpers (DRY)
│      └── Useful functions
│
├── locales
│      └── Translations
│
├── routes
│      └── App routes
│
├── screens
│     └── Screen
│           ├── index.tsx
│           └── styles.tsx
├── services
│      └── Api services (aka: Realm local server)
│
├── styles
│      ├── colors
│      │    └── base app theme
│      │
│      └── baseStyles (DRY)
│
└── index.tsx
```

<br />

## ✨ Used technologies

- React + Hooks
- Typescript
- Styled Components
- Formik
- React Navigation v5
- React Native Testing Library (🦉)
- Prettier
- Eslint
- Realm (Database)

<br />

## TODO

- [ ] Storybook documentation
- [ ] More test coverage
- [ ] CD - Fastlane: https://fastlane.tools
- [ ] CI - Bitrise: https://bitrise.io
- [ ] DRY the code (Don't repeat yourself)

<br />

## 👨‍💻 Contributors

Have a look [here](https://github.com/GleidsonDaniel/transactions-manager/blob/develop/contributing.md) if you want to contribute!

<br />

### ©️ Open source - licence

Repository and contributions are under [GNU General Public License v3.0](https://github.com/GleidsonDaniel/transactions-manager/blob/develop/LICENSE)
