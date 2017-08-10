Car/TransmissionType
==================

**Описание:** Вывод вида коробки авто

**Процедура:** R4_Common..psx_TransmissionType_Select

Запрос:
~~~~~~

::

    POST /api/Car/TransmissionType HTTP/1.1
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
        "msg": "Вывод вида коробки авто",
        "logmsg": null,
        "data": [
            {
                "TransmissionTypeID": 2,
                "TransmissionTypeName": "Автоматическая"
            },
            {
                "TransmissionTypeID": 1,
                "TransmissionTypeName": "Механическая"
            }
        ]
    }