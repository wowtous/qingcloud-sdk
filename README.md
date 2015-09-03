qingcloud-sdk
=============
* A node port of qingcloud.com's NodeJs SDK library.
* The project forks from https://github.com/Pana/qingcloud-sdk

## Example
```
var qing = require('qing');
// set key_id and key
qing.access_key_id = 'access_key_id';
qing.secret_access_key = 'secret_access_key';
// call the API
qing.DescribeInstances({zone: 'pek1'}, function(err, data){
    if(err)
        console.log(err.message);
    else
        console.log(data);
});
```

## 说明

* 私钥id和密匙到控制台中添加查看
* zone参数目前只有'pek1'
* 目前内部使用sha256加密方式
* 带n的参数值必须为数组
* 具体参数参看青云[官方文档](https://docs.qingcloud.com/api/index.html)
