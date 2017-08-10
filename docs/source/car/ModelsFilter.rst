Car/ModelsFilter
==================

**Описание:** Вывод моделей авто

**Процедура:** R4_Common..psx_CarModel_Select

Запрос:
~~~~~~

::

    POST /api/Car/ModelsFilter HTTP/1.1
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
            "CarMarkaID":  12
            }
        ]
    }


Ответ:
~~~~~~
::

    {
        "status": "ok",
        "code": 1,
        "msg": "Вывод моделей авто",
        "logmsg": null,
        "data": [
            {
                "CarModelID": 416,
                "CarModelName": "Trazo"
            },
            {
                "CarModelID": 417,
                "CarModelName": "Viper"
            },
            {
                "CarModelID": 418,
                "CarModelName": "Vision"
            }
        ]
    }