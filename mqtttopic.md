## How do you design MQTT topics and payloads for smart washing machine

1. สถานะเครื่องซักผ้า
    - topic:v1cdti/app/get/1212312121/model-01/sn-001/
    - payload
        - {"STATUS": "POWER ON|START|STOP|FINISHED|POWERED OFF"}
1. เซนเซอร์ภายในเครื่องซักผ้า
    - topic:v1cdti/app/get/1212312121/model-01/sn-001
    - payload
        - {"temperature": "25.2"}
        - {"Pressure": "10bar"}
        - {"3-d Position": "left30"}
        - {"Weight sensor": "50kg"}
        - {"presence detection": "yes"}
        - {"Material detection": "unusual matt"}
        - {"liquid flow": "stable"}
        - {"vibration": "stable"}
        - {"balance": "normal"}
        - {"Air quality": "normal"}
        

 1. เซนเซอร์ภายนอกเครื่องซักผ้า
    - topic:v1cdti/app/get/1212312121/model-01/sn-001
    - payload
        - {"Touch": "command"}
        - {"Hall": "close"}
        - {"drain-pump": "working"}
        - {"Track&count people": "not detect"}
        - {"Gesture": "normal"}
        - {"Voice command": "command"}
        - {"Detect clogged": "normal"}



