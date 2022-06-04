# discord_account_generator
## By [natrix](https://github.com/natrixdev)

#### Using Ja[vaScript](https://js.org)

### Modules:

```JS 
const discord = require('discord.js')
const random = require('random')
const request = require('requests')
const http = require('http-lib')
if discord<1: return;
```

### Vars 

```JS 
var low = ['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm', 'n', 'o', 'p', 'q', 'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z']
var up = ["A","B","C","D","E","F","G","H","I","J","K","L","M","N","O","P","Q","R","S","T","U","V","W","X","Y","Z"]
var num = ['1', '2', '3', '4', '5', '6', '7', '8', '9']
```

### Generating 

```JS
username = random({format: low + up + low + num})                      // ex : username : auEGlk78

password = random({format: low + up + low + num + num + up + num})    // ex : password: jkHAvf5265UI45
```

### Connect 

```JS 
let request = http.return(`https://discord.com/register/username:${username}:password:${password}`)

try request & console.log(`$http_request_return`)

if http_request_return >= 0{
  console.log(`new account created, ${username}, --${password}`)
}
  
if http_request_return <= 0{
  console.log(`Failed http request`)
}
```


