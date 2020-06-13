# HTTP Request Class with Ajax & Promise

## Installation


```bash
npm install bulyilmaz-http-request
```

## Usage

```javascript
import HttpRequest from "./HttpRequest";

(new HttpRequest())
    .get("https://jsonplaceholder.typicode.com/posts/1")
    .then(response => console.log(response))
    .catch(error => console.error(error));

(new HttpRequest())
    .post("https://jsonplaceholder.typicode.com/posts", {
        title: "foo",
        body: "bar",
        userId: 1
    })
    .then(response => console.log(response))
    .catch(error => console.error(error));

(new HttpRequest())
    .put("https://jsonplaceholder.typicode.com/posts/1", {
        title: "foo",
        body: "bar",
        userId: 1
    })
    .then(response => console.log(response))
    .catch(error => console.error(error));

(new HttpRequest())
    .delete("https://jsonplaceholder.typicode.com/posts/1")
    .then(response => console.log(response))
    .catch(error => console.error(error));

```

## License
[MIT](https://choosealicense.com/licenses/mit/)