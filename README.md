# ppposclient
Arduino client library for gsm ppp protocol. This library can be used to make GET and POST requests and to connect mqtt with PubSubClient (https://github.com/knolleary/pubsubclient). It supports ESP32 (tested with version 2.0.0).

# VSCode + PlatformIO 환경에서 ESP32 코어 버전(tested with version 2.0.0)을 맞추려면
set 'platformio.ini'  
platform = espressif32@4.0.0

# 리포지토리 목적
codezoo/ppposclient 라이브러리의 MQTT 연결 실패 후 연결 회복이 잘 안되는 문제 및  
ppposclient 라이브러리를 VSCode + PlatformIO 환경에서 빌드 시 'fd()' 메소드 참조 문제 발생으로  
사용자 편의를 위해 ppposclient 라이브러리를 fork + customize 하였습니다.

# 변경점
1. 최신화: 원본인 levkovigor/ppposclient를 fork
2. codezoo 커스텀: codezoo/ppposclient에서 포팅/추가된 내용 merge
3. fd() 메소드 참조 문제: 주석처리 (로깅 코드라 큰 지장은 없어보입니다.)

원본: https://github.com/levkovigor/ppposclient  
codezoo: https://github.com/codezoo-ltd/ppposclient)

![CATM1_embedded_Modem](https://user-images.githubusercontent.com/22319034/154849388-0d8e82a9-f7bd-42d2-b8d9-fb31798dc67e.png)

# Blog Story
https://codezoo.tistory.com/28
