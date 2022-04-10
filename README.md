# crud-http-frontend
Simplest Tool to Talk with REST API's in HTML (wrapper for axios)

### Example:
```
<div id="reponse"></div>

<script src="axios.min.js"></script>
<script src="crud-http.js"></script>
<script>
    let url = 'http://localhost:5684/api'; // replace with your API
    let promise = http_read(url);
    promise.then((data) => {
        let element = document.getElementById("reponse");
        element.innerHTML = JSON.stringify(data);
    });
</script>
```

### Methods
```
let promise = http_create(url,data,authValue=null); // authValue sets "Authorization" header for account specific actions
let promise = http_read(url,authValue=null); // authValue sets "Authorization" header for account specific actions
let promise = http_update(url,data,authValue=null); // authValue sets "Authorization" header for account specific actions
let promise = http_delete(url,authValue=null); // authValue sets "Authorization" header for account specific actions
``` 

### Installation
Download axios.min.js and crud-http.js, and store them in your public folder.

On Linux:
```
cd /var/www/html/your-project
git clone https://github.com/neil-yoga/crud-http-frontend
mv crud-http-frontend/*.js .
```

