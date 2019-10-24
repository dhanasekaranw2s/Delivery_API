# Task Creation

Task Creation Api.

**URL** : `/api/new_order/`

**Method** : `POST`

**Auth required** : Yes

**Headers required**:

 ```x-client-data: <client_token>```

 ```x-client-date: <Current_Time_String>```

```Authorization: <auth_token>```


**Data constraints**

```json
{
    "cust_email":"ReceiverEmail@mail.com",
    "geo_fence_meter":200,
    "sender_name":"test",
    "sender_number":"+919876543210",
    "sent_ladd":12.948247,
    "sent_long":80.210062,
    "data":{
        "cust_address":"Fish Market, Vembuli Amman Koil Street, Seevaram, Thoraipakkam, Chennai, Tamil Nadu, India",
        "cust_email":"ReceiverEmail@mail.com",
        "cust_name":"Receiver Second",
        "cust_phone":"+911234567899",
        "geo_fence_meter":200,
        "is_geo_fence":1,
        "loc_lat":"12.951622623567",
        "loc_lng":"80.241289428836",
        "method":"Pickup",
        "notes":"test",
        "order_id":"123",
        "pick_address":"W2S Solutions - Mobile (Android & iPhone) Application Development Company - Software Development, 200 Feet Radial Road, Sri Sai Nagar, Thoraipakkam, Chennai, Tamil Nadu, India",
        "pick_date_time":"2019-10-18 20:20",
        "picktime":"2019-10-18T12:50:00.000Z",
        "pickup_ladd":12.94996,
        "pickup_long":80.23772800000006,
        "schedule":"2019-10-18T13:10:00.000Z",
        "schedule_date_time":"2019-10-18 20:40",
        "sender_name":"test",
        "sender_number":"+919876543210",
        "sent_address":"Kamatchi Hospital, Ma Po Si Nagar, Pallikaranai, Chennai, Tamil Nadu",
        "sent_ladd":12.948247,
        "sent_long":80.210062,
        "showdeliv":false,
        "showpick":false,
        "status":"Unallocated",
        "type":0
    }
}


```

**Data example**

```json
{
    "cust_email":"ReceiverEmail@mail.com",
    "geo_fence_meter":200,
    "sender_name":"test",
    "sender_number":"+919876543210",
    "sent_ladd":12.948247,
    "sent_long":80.210062,
    "data":{
        "cust_address":"Fish Market, Vembuli Amman Koil Street, Seevaram, Thoraipakkam, Chennai, Tamil Nadu, India",
        "cust_email":"ReceiverEmail@mail.com",
        "cust_name":"Receiver Second",
        "cust_phone":"+911234567899",
        "geo_fence_meter":200,
        "is_geo_fence":1,
        "loc_lat":"12.951622623567",
        "loc_lng":"80.241289428836",
        "method":"Pickup",
        "notes":"test",
        "order_id":"123",
        "pick_address":"W2S Solutions - Mobile (Android & iPhone) Application Development Company - Software Development, 200 Feet Radial Road, Sri Sai Nagar, Thoraipakkam, Chennai, Tamil Nadu, India",
        "pick_date_time":"2019-10-18 20:20",
        "picktime":"2019-10-18T12:50:00.000Z",
        "pickup_ladd":12.94996,
        "pickup_long":80.23772800000006,
        "schedule":"2019-10-18T13:10:00.000Z",
        "schedule_date_time":"2019-10-18 20:40",
        "sender_name":"test",
        "sender_number":"+919876543210",
        "sent_address":"Kamatchi Hospital, Ma Po Si Nagar, Pallikaranai, Chennai, Tamil Nadu",
        "sent_ladd":12.948247,
        "sent_long":80.210062,
        "showdeliv":false,
        "showpick":false,
        "status":"Unallocated",
        "type":0
    }
}

```



## Success Response

**Code** : `200 OK`

**Content example**

```json

{
    "data": "Task Created",
    "status": "ok"
}


```

## Error Response

**Content** :

```json
{
    "data": "<Error Msg>",
    "status": "error"
}
```
