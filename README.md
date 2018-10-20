# manjaroSettingDocuments
아치리눅스 만자로 배포판 정리

## 배포판 선택
-> [Manjaro XFCE Edition](https://osdn.net/dl/manjaro/manjaro-xfce-17.1.12-stable-x86_64.iso) : lightweight desktop environment(개인적으로 깔끔하다 생각)

## 유용한 유틸리티
### [rofi](https://github.com/DaveDavenport/rofi)
스팟라이트/alfred와 같은 간단 런처
```
$ sudo pacman -S rofi
```
### [zeal](https://github.com/zealdocs/zeal)
오프라인 도큐먼트 문서. dash for mac과 같다. \
Qt관련 버그가 있는듯. 예전엔 HiDPI 관련 이슈로 아이콘등이 이상하게 크기가 이상하더니, 아에 구동이 안되기도 한다.\

github에서 직접 소스를 받아 빌드하여 실행하고, 쉘 스크립트 신공으로 실행토록 ㅏㄴ다.ㅎ
```
$ git clone https://github.com/zealdocs/zeal
$ cd zeal
$ mk build && cd build
$ cmake ..
$ make && sudo make install

$ sudo vi /usr/bin/launchZeal

---
#!/bin/sh
QT_AUTO_SCREEN_SCALE_FACTOR=0 zeal
---
// 저장 후 
$ sudo chmod+x /usr/bin/launchZeal
// 앞으로 launchZeal로 실행이 가능하다.

```
### 한글입력기 [Nimf](https://github.com/janghe11/nimf)
이게 제일 나은듯\
```
$ yaourt -s nimf
```


