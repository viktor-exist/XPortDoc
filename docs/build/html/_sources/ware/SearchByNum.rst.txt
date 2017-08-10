Ware/SearchByNum
==================

**Описание:** Метод получает список товаров по поисковому значению

**Процедура:** R4_TMC..psx_Ware_SearchByNum

Запрос:
~~~~~~

::

    POST /api/Car/SimpleQueryVIN HTTP/1.1
    Host: testxport.exist.ua:14088
    Content-Type: application/json
    Authorization: Basic {{логин/пароль в base64}}
    {
    "msg": "пример",
    "parameters": [
        {
        "VinCode": "testVIN",
        "MarkaID": "207",
        "ModelID": "1178",
        "Size": "1,4 16V",
        "YearRelease": "2002",
        "FuelTypeID": "1",
        "TransmissionTypeID": "2",
        "Email": "test@test.mail",
        "SendEmail": "on",
        "Wares": {
            "Item": ["Ware 1","Ware 2","Ware 3"]
        },
        "SessionID": 10816197
        }
    ]
    }


Ответ:
~~~~~~
::

    {
    "status": "ok",
    "code": 1,
    "msg": "Выборка по номеру",
    "data": [
        {
        "TypeRecord": 2,
        "WareId": 11303727,
        "WareNum": "LF3376",
        "WareName": "Масляный фильтр",
        "TradeMarkID": 2908,
        },
        {
        "TypeRecord": 3,
        "WareId": 11657672,
        "WareNum": "WL7135",
        "WareName": "Масляный фильтр",
        "TradeMarkID": 4331,
        "TradeMarkName": "WIX",
        }
    ]
    }

        
