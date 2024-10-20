# 7segment-Arduino-Shield-TM1630  
https://massa4649.booth.pm/items/6125310 の製品説明となります。  

## 概要
Arduinoにスタックして動かせるキースキャン機能付き4桁7セグメントLEDシールドです。  
  
![IMG_1151-30per](https://github.com/user-attachments/assets/c17356ec-72f0-4059-a0ca-44589f4c1a2f)  

## バリエーション  
・基板のみ必要な方向けの【基板単品】と、必要部品をまとめた【部品キット】を準備しました。  
　完成形にする場合は、【基板単品】と【部品キット】の両方が必要です。  

### 【基板単品】
・両面基板仕様  １枚　サイズ(typ)：53.3 x 68.6 x 1.6 mm  
![gaikan-30per](https://github.com/user-attachments/assets/4d004dea-707f-4d60-9945-f83406144a12)  

### 【部品キット】
・下記が同梱されています。  
||部品名|個数|備考|
|-----|-----|-----|-----|
|1|7セグメントLED(右dot)|４個|HP5082-7760|
|2|LEDドライバーIC|１個|TM1630|
|3|タクトスイッチ|６個|6.5×4.5mmピッチ品|
|4|６ピンソケット|１個|2.54mmピッチのピンソケット|
|5|８ピンソケット|２個|2.54mmピッチのピンソケット|
|6|１０ピンソケット|１個|2.54mmピッチのピンソケット|
|7|ダイオード|６個|キー同時押し時のSEGピンショート防止用|
|8|10k ohm 抵抗|３個|１６０８サイズ|  
|9|100pFコンデンサ|３個|１６０８サイズ|  
|10|1nFセラミックコンデンサ|１個|挿入タイプ|  
|11|10uF電解コンデンサ|１個|挿入タイプ|  

※オプション回路の８ピンソケット(J6)、３ピンヘッダ(J5)、ジャンパピン(J5用)、10kΩ抵抗×2個(R4,R5) はキットに含まれません。  
※ロットにより、部品名称や色あい、細かいデザインや形が微妙に変わることがあります。  

## 回路図  
![4DIGIT-7SEGーLED_TM1630](https://github.com/user-attachments/assets/7ca48a51-4511-45d0-821b-cdc8e82f12c8)

2024年10月現在においては、TM1630は電子部品ショップの秋月電子さんでも販売されていますので、そちらのWEBサイトにデータシートがありますのでご参照下さい。  
TOPページ：https://akizukidenshi.com/catalog/c/c0/  
販売コード：113223  

## 動作確認
・Arduino.ccサイトでリファレンス紹介されている”TM16xx LEDs and Buttons”ライブラリを使用して動作確認をしました。  
　サイト：https://reference.arduino.cc/reference/en/libraries/tm16xx-leds-and-buttons/  
　ただし、オリジナルでは、4桁の消去が上手くできなかったため、TM1630.cpp　ファイルの一部を下記の赤丸のように変更しました。  

![cppファイル-50per](https://github.com/user-attachments/assets/d07a6450-0f7e-4b05-9a49-de5a71972214)  

### 動画  
[![紹介動画]()](https://youtu.be/ZaXRua2_uDM)  

## 関連ブログ
https://massa4649.com/tm1630_1/

以上です。
