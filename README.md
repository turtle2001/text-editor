# Text Editor

## Description

This goal of this project is to create a text editor that is a progressive web application. The app allows you to take notes on or offline.

Technologies Used

[Deployed App]()

## Installation

Dependencies can be installed by using the following command:

```sh
npm install
```

Start it up with

```sh
npm run start
```

## Code Snippet

This adds content to the database

```js
export const putDb = async (content) => {
  const contactDb = await openDB('jate', 1);
  const tx = contactDb.transaction('jate', 'readwrite');
  const store = tx.objectStore('jate');
  const request = store.put({ id: 1, value: content });
  const result = await request;
  console.log('Data saved', result);
};
```

## Author Links

[LinkedIn](https://www.linkedin.com/in/alexis-zaragoza-5baa51242/)
[GitHub](https://github.com/turtle2001)
