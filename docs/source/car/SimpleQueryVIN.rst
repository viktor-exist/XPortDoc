Car/SimpleQueryVIN
==================

**Описание:** Запись по запросу VIN

**Процедура:** R4_Order..psx_SimpleQueryVIN_Create

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
   
