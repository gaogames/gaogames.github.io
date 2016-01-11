---
layout:     post
title:      "본 쉘(Bourne Shell): /bin/sh"
date:       2016-01-11
author:     Eric Kang
summary:    본쉘에 대해 간략히 설명한다.
categories: Linux
thumbnail:  heart
tags:
 - linux
 - shell
 - bourne shell
---
주제는 본쉘이지만 대부분의 리눅스 배포판의 기본쉘인 bourne-again shell(bash)를 기준으로 설명합니다.

## 쉘 프롬프트

터미널로 접속해서 볼 수 있는 프롬프트의 모양은 환경변수 `PS1` 을 따릅니다. 자신의 현재 프롬프트 설정은 다음의 명령어로 확인할 수 있습니다.


```
$ echo $PS1
```

`$HOME/.bashrc` 파일에 다음과 같은 줄을 추가해서 프롬프트의 모양을 바꿔봅시다.

```
PS1="[\u@\h \W]\\$ "
```

