---
title: Project Progress 1/22/2020
description: 1/22/2020의 프로젝트 진행사항 LoRa 게이트와 LoRa 쉴드를 이용해서 데이터 취합을 하는 것과 또 다른 LoRa 쉴드를 이용해서 API로 water pump를 제어할 수 있도록 코드를 작성하였다.
categories:
 - Project
tags: LoRa
---


## LoRa 통신
LoRa gateway와 LoRa Shield를 네트워크를 연결하는 코드를 완성하였다. LoRa shield & arduino에서 얻은 센서값 온도, 습도, 토양습도를 LoRa gateway에 전송한다. LoRa gateway는 인터넷과 연결되어있어서 Thingspeak에 센서값을 전송하여 저장한다.

## LoRa 컨트롤
LoRa gateway에는 내장 웹서버를 가지고 있어서 Bridge라는 모듈을 통해 REST API를 이용할 수 있다. 이제 백엔드 서버에서 water pump를 제어할 수 있게 되었다.

## After
water pump를 언제 열고 닫을지 옥수수의 생육 조건과 기후조건을 생각해서 언제 water pump를 언제 열고 닫을지 결정을 해야 겠다.
날씨  기후 조건에 대해서는 ml도 생각 중이다.