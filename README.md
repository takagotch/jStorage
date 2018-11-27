### jStorage
---
https://github.com/andris9/jStorage

```jq
$.jStorage.set(key, value, options)
$.jStorage.deleteKey(key)
$.jStorage.set("mykey", "keyvalue");
$.jStorage.setTTL("mykey", 3000);
$.jStorage.flush()
$.jStorage.index()
$.jStorage.storageSize()
$.jStorage.currentBackend()
$.jStorage.reInit()
$.jStorage.storageAvailable()
$.jStorage.subscribe("ch1", function(channel, payoad){
  console.log(payload+ " from" + channel);
});
$.jStorage.publish("ch1", "data");
$.jStorage.listenKeyChange("mykey", function(key, action){
  console.log(key + " has been " + action);
});
$.jStorage.listenKeyChange("*", function(key, action){
  console.log(key + " has been " + action);
});
$.jStorage.stopListening("mykey");
```

```js
value = $.jStorage.get(key)
value = $.jStorage.get(key, "default value")

ttl = $.jStorage.getTTL("mykey");
var index = $.jStorage.index();
console.log(index);
```

```
```

