# crud-http-frontend
Simplest REST API Util (wrapper for axios)

Example:
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
      
    // optional error handling
    promise.catch((err) =>{
        let element = document.getElementById("reponse");
        element.innerHTML = JSON.stringify(err);
    });
</script>
```

#### Methods
```
let promise = http_create(url,data,authValue=null); // authValue sets "Authorization" header for account specific actions
let promise = http_read(url,authValue=null); // authValue sets "Authorization" header for account specific actions
let promise = http_update(url,data,authValue=null); // authValue sets "Authorization" header for account specific actions
let promise = http_delete(url,authValue=null); // authValue sets "Authorization" header for account specific actions
``` 


