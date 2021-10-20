# BLE_Uart iOS App과 Board의 firmware
- 디바이스의 경우 [Adafruit Bluefruit LE SPI Friend 보드](https://learn.adafruit.com/introducing-the-adafruit-bluefruit-spi-breakout?view=all)를 사용
- iOS앱의 경우 [이 문서](https://learn.adafruit.com/build-a-bluetooth-app-using-swift-5?view=all)를 참고
- UART서비스의 서비스 UUID는 다음과 같다.

```C++
const serviceUuid = "6e400001-b5a3-f393-e0a9-e50e24dcca9e";
```
- UUID의 영문은 소문자이고, 웹(Web BLE)에서 사용을 할때 일부 UUID는 gatt blocklist에 있어서 사용할 수 없음. (다음 링크 참고)
- https://github.com/WebBluetoothCG/registries/blob/master/gatt_blocklist.txt
