###简要描述：

- 幻灯片查询接口

###请求URL：

- `/datahandler/customerapp/appslider/findbymap`
  
###请求方式：

- POST 

###参数：

|参数名|必选|类型|说明|demo|
|:----|:---|:----- |-----   |
|cityCode|是  |String |高德地图城市编码(如南京市-025)|025|
|modelId|是  |String |幻灯模板id 1：客户端首页幻灯组（目前业务只传1）|1|

###返回code：

|值|说明|
|:----|:-----|
|6000| 数据请求成功 |
|7000| 返回列表为空，业务逻辑错误 |
|7003| 数据请求失败 |
###返回data：

|key|说明|demo|
|:----|:-----|:-----|
|id| 自增id |876 |
|name|幻灯片名称 |首页顶部幻灯1|
|modelId|幻灯模板id |1 |
|platform|平台标识（客户端app 0：全平台 1：仅android 2:仅ios 3.仅winPhone）|0|
|cityCode|高德城市编码|025|
|imgUrl|图片Url |f3114e86976037e75ff9bcb44dca424f|
|modelName|幻灯片组名称 |首页幻灯|
|silderParams|幻灯片调整参数（预留） | |
|sortOrder|排序依据|1|
|operateUser|操作人Id|e623bfe960e241ee9449fa353b0fae81|
|status|状态值 0：正常 -1：停用|0|
###返回示例：

```
{
    "code": "6000",
    "exceptions": null,
    "data": [
        {
            "id": 1,
            "name": "首页顶部幻灯1",
            "modelId": 1,
            "platform": "0",
            "cityCode": "Magugi",
            "imgUrl": "f3114e86976037e75ff9bcb44dca424f",
            "silderParams": " ",
            "modelName": "首页幻灯",
            "status": "0",
            "sortOrder": "1",
            "operateUser": "初始化"
        },
        {
            "id": 2,
            "name": "首页顶部幻灯2",
            "modelId": 1,
            "platform": "0",
            "cityCode": "Magugi",
            "imgUrl": "1fd939f3bc22462f62b85d55e9946970",
            "silderParams": " ",
            "modelName": "首页幻灯",
            "status": "0",
            "sortOrder": "2",
            "operateUser": "初始化"
        },
        {
            "id": 3,
            "name": "首页顶部幻灯3",
            "modelId": 1,
            "platform": "0",
            "cityCode": "Magugi",
            "imgUrl": "13a98be90c9048ce8786ec9b05cef88f",
            "silderParams": " ",
            "modelName": "首页幻灯",
            "status": "0",
            "sortOrder": "3",
            "operateUser": "初始化"
        },
        {
            "id": 4,
            "name": "首页顶部幻灯4",
            "modelId": 1,
            "platform": "0",
            "cityCode": "Magugi",
            "imgUrl": "7d8a6458da570bbab72c9c95924a5794",
            "silderParams": " ",
            "modelName": "首页幻灯",
            "status": "0",
            "sortOrder": "4",
            "operateUser": "初始化"
        },
        {
            "id": 5,
            "name": "首页顶部幻灯5",
            "modelId": 1,
            "platform": "0",
            "cityCode": "Magugi",
            "imgUrl": "c2f72c332b54d52326b2b7f0e0e45051",
            "silderParams": " ",
            "modelName": "首页幻灯",
            "status": "0",
            "sortOrder": "5",
            "operateUser": "初始化"
        }
    ]
}
```
###接口负责人：
- Issac