Car/FuelType
==================

**Описание:** Вывод типа топлива авто

**Процедура:** R4_Common..psx_FuelType_Select

Запрос:
~~~~~~

::

    POST /api/Car/FuelType HTTP/1.1
    Host: testxport.exist.ua:14088
    Content-Type: application/json
    Authorization: Basic {{логин/пароль в base64}}
    {
        "role": "admin",
        "msg": "пример",
        "lang":"ru",
        "version": 1,
        "parameters": [
            {
            
            }
        ]
    }

Ответ:
~~~~~~
::

    {
        "status": "ok",
        "code": 1,
        "msg": "Вывод типа топлива авто",
        "logmsg": null,
        "data": [
            {
                "FuelTypeID": 1,
                "FuelTypeName": "Бензин"
            },
            {
                "FuelTypeID": 4,
                "FuelTypeName": "Иное"
            }
        ]
    }