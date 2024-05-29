![alt text](OIP.jpg)

# Что такое Axios в JS ?

## Axios - это библиотека JavaScript, которая позволяет делать HTTP-запросы из браузера или из Node.js. Она предоставляет простой и удобный интерфейс для выполнения запросов на сервер и обработки ответов !

## Вот некоторые особенности Axios : <br> 1. Изоморфность: Axios может работать как в браузере, так и в Node.js, используя одну и ту же базу кода. <br> 2. Promise API: Он поддерживает промисы, что делает его удобным для асинхронных операций. <br> 3. Автоматическое преобразование JSON-данных: Axios автоматически преобразует данные запроса и ответа в формат JSON. <br> 4. Поддержка перехвата запросов и ответов: Вы можете перехватывать запросы и ответы для дополнительной обработки. <br> 5. Отмена запросов: Axios позволяет отменять запросы, если это необходимо.

## Для подключения Axios вы можете использовать <script> то есть через 

```js
<script src="https://cdn.jsdelivr.net/npm/axios/dist/axios.min.js"></script>
```

...

# Axios , Get :

```js
async function getData() {
  try {
    const { data } = await axios.get(api);
    get(data);
  } catch (error) {
    console.error(error);
  }
}

getData();
```

...

# Axios , Post :

```js
async function postUser(user) {
  try {
    const { data } = await axios.get(api, user);
    getData();
  } catch (error) {
    console.error(error);
  }
}
```

# Axios , Put : 

```js
async function putUser(id, user) {
  try {
    const { data } = await axios.put(`${api}/${id}`, user);
    getData();
  } catch (error) {
    console.error(error);
  }
}
```

