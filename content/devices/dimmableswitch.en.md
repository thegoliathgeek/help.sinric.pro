---
title: "Dimmable Smart Socket"
date: 2019-06-15T11:02:05+06:00
type: "post"
author: "Aruna"
---
 
The following shows an example of how to use a smart switch device.

Login to [Sinric] (https://sinric.pro) and create a "Dimmable Switch" device.

Copy the API key and device Id and update the sketch like below.

```toml
    ....
    webSocket.setAuthorization("apikey", MyApiKey);
    ....
```

<b>Turn On</b> command 
    
```toml
   {
        "clientId":"android-app",
        "did":"xxxxxx",
        "type":"action",
        "ts":"1556844829681",
        "actions":[
            {"name":"setOn","parameters":{}}
        ]
   }
```

<b>Turn Off</b> command 
    
```toml
   {
        "clientId":"android-app",
        "did":"xxxxxx",
        "type":"action",
        "ts":"1556844829681",
        "actions":[
            {"name":"setOff","parameters":{}}
        ]
   }
```

<b>Dim</b> command 

Examples: <br>
Alexa, set the power to 40 percent on the fan.



```toml
   {
        "clientId":"android-app",
        "did":"xxxxxx",
        "type":"action",
        "ts":"1556844829681",
        "actions":[
            {
              "name":"setPowerLevel", 
              "parameters": {
                  "value" : 60
                }
            }
        ]
   }
```


it's that simple. 


<!-- Just download latest version of [Hugo binary (> 0.53)](https://gohugo.io/getting-started/installing/) for your OS (Windows, Linux, Mac) : it's that simple. 

![image example](../../../../images/hugo.jpg "image")
-->