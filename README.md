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

### Bonus: Keep things alive
```
// Enjoy the free code sharing. 
//
// ☯️ If you used my code to save time,
//  consider donating eco-friendly crypto:
```

```
nano_3boxqk5q56xsz8ufrw9srrz4pta6ffbkrg9j31aqziz8wtnr6j68ci7s4cnc
```

```
// It matters: Everything is an energy exchange ⚡.
//
//
// ^ Also feel free to copy this template for your own projects and replace the wallets.
// 🙏 You deserve to be happy and free.
```

### Nano?
<a style="color:black;font-size:15px;" href="https://nano.org">Zero Fees, Eco-Friendly, Instant Payments</a>

