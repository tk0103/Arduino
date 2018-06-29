## 概要
* 部屋にあるリモコンを統一。TV、扇風機、エアコン

## 部品
* 赤外線リモコン受信モジュール(I-00614)
* 赤外線LED OS15LA5113A(I-12612)
* トグルスイッチ
* 抵抗

## 通信フォーマット
http://elm-chan.org/docs/ir_format.html


## 解析結果
* Hisense製TV(NECフォーマット)、カスタマーコード16bit(0x00,0xbf)
* データコード：8bitのデータと8bitの反転データ
* 扇風機、カスタマーコード16bit(0x06,0xa3)
* データコード：8bitデータ共通(0x70) + 8bitデータ  

|ボタン(TV)|データコード|ボタン(Fan)|データコード|
|:---:|:---:|:---:|:---:|
|Power|0x0d|Power|0xe0|
|入力切替|0x12|風量|0x00|
|1|0x01|首振り|0x80|
|2|0x02|切タイマー|0x40|
|3|0x03|入タイマー|0x20|
|4|0x04|
|5|0x05|
|6|0x06|
|7|0x07|
|8|0x08|
|9|0x09|
|10|0x00|
|11|0x0b|
|12|0x1c|
|↑|0x16|
|→|0x18|
|↓|0x17|
|←|0x19|
|番組表|0x1d|
|決定|0x15|
|戻る|0x48|
|メニュー|0x14|
|サブメニュー|0x4f|
|VOLUME UP|0x44|
|VOLUME DOWN|0x43|
|CH UP|0x4a|
|CH DOWN|0x4b|
|早戻し|0x57|
|再生|0x1e|
|早送り|0x56|
|一時停止|0x4e|
|見る|0x5d|


## Image
|実装|
|---|
|<img src="" alt="test" title="test" width="473" height="336">|


