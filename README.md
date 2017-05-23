
**请求URL：** 
- ` http://xx.com/_API/_getAssociation?userId=1&timestamp=14XXXXXX&sign=s15f1s56fa1sd5fsadfaxzfwewe `
  
**请求方式：**
- GET 

**参数：** 

|参数名|必选|类型|说明|
|:----    |:---|:----- |-----   |
|userId |是  |int | 用户Id    |

 **返回示例**

```
{
    "error_code": "E0000",
    "data": [
        {
            "id": "22",
            "is_apply": 2,
            "owner_id": "16",
            "group_id": "16894435328001",
            "name": "baidu",
            "level": "1",
            "bulletin": " ",
            "pri_url": "http://192.168.1.250:8099/images/default/108-01.png",
            "current_number": "1",
            "max_number": "50"
        },
        {
            "id": "13",
            "is_apply": 2,
            "owner_id": "10",
            "group_id": "16831168446465",
            "name": "qweqweqwe",
            "level": "1",
            "bulletin": " ",
            "pri_url": "http://192.168.1.250:8099/images/default/108-01.png",
            "current_number": "2",
            "max_number": "50"
        },
        {
            "id": "21",
            "is_apply": 2,
            "owner_id": "15",
            "group_id": "16893791502337",
            "name": "baidu.com",
            "level": "1",
            "bulletin": " ",
            "pri_url": "http://192.168.1.250:8099/images/default/108-01.png",
            "current_number": "1",
            "max_number": "50"
        },
        {
            "id": "1",
            "is_apply": 2,
            "owner_id": "3",
            "group_id": "16795311341569",
            "name": "ccc",
            "level": "1",
            "bulletin": " ",
            "pri_url": "http://192.168.1.250:8099/images/default/10.png",
            "current_number": "2",
            "max_number": "50"
        },
        {
            "id": "19",
            "is_apply": 2,
            "owner_id": "11",
            "group_id": "16893574447105",
            "name": "asdfew",
            "level": "1",
            "bulletin": " ",
            "pri_url": "http://192.168.1.250:8099/images/default/108-01.png",
            "current_number": "1",
            "max_number": "50"
        },
        {
            "id": "20",
            "is_apply": 2,
            "owner_id": "14",
            "group_id": "16893761093633",
            "name": "www",
            "level": "1",
            "bulletin": " ",
            "pri_url": "http://192.168.1.250:8099/images/default/108-01.png",
            "current_number": "1",
            "max_number": "50"
        }
    ]
}
```

 **返回参数说明** 

|参数名|类型|说明|
|:-----  |:-----|-----                           |
|error_code |string   |error_code错误代码  |
|data|array|返回数据  如果用户加入公会第一条数据则是用户所在公会|
|myAssociation|array|我的公会|
|list|array|公会列表|
|-|-|-|
|is_apply|int|是否申请该公会   1:已申请   2:未申请|
|id|int|公会id|
|owner_id|int|公会会长ID|
|group_id|bigint|环信群组id|
|name|string|公会名称|
|level|int|公会等级|
|bulletin|string|公会公告|
|pri_url|string|公会头像地址|
|current_number|int|公会当前成员数|
|max_number|int|公会上限成员数|
 

 **备注** 
- 登陆之后的所有操作必须按照规定方法对参数做签名和处理，详情请看首页【接口调用方法】。
- 更多返回错误代码请看首页的错误代码描述。


