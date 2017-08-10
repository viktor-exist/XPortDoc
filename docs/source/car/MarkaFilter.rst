Car/MarkaFilter
==================

**Описание:** Вывод марок авто

**Процедура:** R4_Common..psx_CarMarka_Select

Запрос:
~~~~~~

::

    POST /api/Car/MarkaFilter HTTP/1.1
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
