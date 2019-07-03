---
title: "Smart Light Bulb"
date: 2018-12-29T11:02:05+06:00
type: "post"
weight: 1
---


The following shows an example of how to use a smart switch device.

Login to [Sinric] (https://gohugo.io/getting-started/installing/) and create a "Switch" device.

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


it's that simple. 


<!-- Just download latest version of [Hugo binary (> 0.53)](https://gohugo.io/getting-started/installing/) for your OS (Windows, Linux, Mac) : it's that simple. 

![image example](../../../../images/hugo.jpg "image")
-->