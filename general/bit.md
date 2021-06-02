# Bit

컴퓨터는 0과 1로 이루어진 정보를 처리합니다.
컴퓨터가 처리하는 가장 작은 단위를 비트(bit)라고 합니다.

| bit  |     cases      |  number  |
| :--: | :------------: | :------: |
| 1bit |      0, 1      |  2(2^1)  |
| 2bit | 00, 01, 10, 11 |  4(2^2)  |
| 3bit |      ...       |  8(2^3)  |
| ...  |      ...       |   ...    |
| 8bit |      ...       | 256(2^8) |

일반적으로 바이트(byte)라는 말을 많으쓰며, 1byte 는 8bit 입니다.

## Unit

1KB = 1024 Byte = 2^10 bytes
1MB = 1024 KByte = 2^20 bytes
1GB = 1024 MByte = 2^30 bytes
1TB = 1024 GBtye = 2^40 bytes

## ASCII

- 컴퓨터에서 문자를 표현하려면 숫자를 이용해야 하는데, 이때 문자 표현을 위한 약속들 중 한 가지가 아스키코드입니다.
- 미국표준협회(ANSI: American National Standards Institute)에 의해서 정의되었습니다.
- 1byte로 표현되었습니다
- 다국어를 표현하기에는 부족합니다

```javascript
String.fromCharCode(65);
// -> A
```

## Unicode

- 2bytes 또는 그 이상으로 이루어진 코드입니다
- 다양한 언어를 표현할 수 있습니다

## Text Encoding

- UTF-8 : Unicode Transformation for mat(8 bit)
- UTF-8은 가변길이 유니코드 인코딩 방식입니다
- UTF-8은 1byte로 표현 가능할 경우 1byte를 사용합니다
- UTF-16 : 기본적으로 2bytes를 사용합니다(1byte로 표현이 가능하더라도 2bytes를 사용합니다)
