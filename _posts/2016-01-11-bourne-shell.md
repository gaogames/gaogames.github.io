---
layout:     post
title:      "본 쉘(Bourne Shell): /bin/sh"
date:       2016-01-11
author:     Eric Kang
summary:    본쉘에 대해 간략히 설명한다.
categories: Linux
thumbnail:  gears
tags:
 - linux
 - shell
 - bourne shell
---
쉘은 사용자가 입력하는 명령을 실행하는 프로그램입니다. 리눅스를 다루기 위해 처음 접하는 것이 쉘이기도 합니다. 앞으로 여러 명령어에 대해 설명할텐데요, 이 명령어들을 모두 쉘에서 입력하면 됩니다.

최근 리눅스 배포판은 대부분 bash(bourne-again shell)이 기본 쉘로 설정돼 있습니다. 이는 좀 더 보강된 본 쉘이라고 보면 됩니다. 앞으로 설명하는 예는 bash 환경입니다.

## 쉘 프롬프트

터미널로 접속해서 볼 수 있는 프롬프트의 모양은 환경변수 `PS1` 을 따릅니다. 자신의 현재 프롬프트 설정은 다음의 명령어로 확인할 수 있습니다.


``` bash
$ echo $PS1
```

`$HOME/.bashrc` 파일에 다음과 같은 줄을 추가해서 프롬프트의 모양을 바꿔봅시다.

``` bash
PS1="[\u@\h \W]\\$ "
```

