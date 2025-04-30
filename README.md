# 적외선 체온계 제작 프로젝트

## 시연영상 링크
https://www.youtube.com/watch?v=NoWK0tbIbYQ


## Blinky Mbed OS example
![](./resources/official_armmbed_example_badge.png)

# Mbed OS Blinky 예제

[![라이선스](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE)

이 예제 프로젝트는 Arm Mbed OS 공식 예제 중 하나로, Mbed OS 입문용 예제입니다. 지원되는 Mbed 보드에서 LED를 반복적으로 깜빡이는 애플리케이션을 포함하고 있습니다.

모든 지원되는 Mbed OS 빌드 도구로 이 프로젝트를 빌드할 수 있지만, 이 프로젝트는 특히 명령줄 인터페이스 도구인 Arm Mbed CLI를 참조합니다.

> **참고**: Arm 온라인 컴파일러로 가져올 수 있는 예제를 보려면 [가져오기 빠른 시작](https://os.mbed.com/docs/mbed-os/latest/quick-start/online-with-the-online-compiler.html)을 참조하세요.

## 요구사항

* [Mbed CLI](https://os.mbed.com/docs/mbed-os/latest/tools/developing-mbed-cli.html) - 버전 1.8.0 이상

## 가져오기

### 방법 1: Git 저장소 복제
```bash
git clone git@github.com:armmbed/mbed-os-example-blinky
cd mbed-os-example-blinky
```

### 방법 2: Mbed CLI 사용
```bash
mbed import mbed-os-example-blinky
cd mbed-os-example-blinky
```

## 애플리케이션 기능

`main()` 함수는 애플리케이션의 단일 스레드입니다. 이 함수는 보드의 LED에 연결된 디지털 출력의 상태를 토글합니다.

## 빌드 및 실행

1. USB 케이블을 사용하여 보드의 USB 포트와 호스트 컴퓨터를 연결합니다.

2. 다음 명령어를 실행하여 예제 프로젝트를 빌드하고 마이크로컨트롤러 플래시 메모리에 프로그래밍합니다:

    ```bash
    mbed compile -m <TARGET> -t <TOOLCHAIN> --flash
    ```

바이너리는 `./BUILD/<TARGET>/<TOOLCHAIN>/mbed-os-example-blinky.bin`에 위치합니다.

또는 USB를 통해 호스트 컴퓨터에 마운트된 보드에 바이너리를 수동으로 복사할 수도 있습니다.

타겟에 따라 GCC_ARM, ARM 또는 IAR 툴체인으로 예제 프로젝트를 빌드할 수 있습니다. Arm Mbed CLI를 설치한 후 다음 명령어를 실행하여 타겟이 지원하는 툴체인을 확인할 수 있습니다:

```bash
mbed compile -S
```

## 예상 결과

보드의 LED가 0.5초(500밀리초) 간격으로 켜지고 꺼집니다.

## 문제 해결

문제가 발생하면 [문서](https://os.mbed.com/docs/mbed-os/latest/tutorials/debugging.html)에서 발생 가능한 문제와 해결 방법에 대한 제안을 검토할 수 있습니다.

## 관련 링크

* [Mbed OS 통계 API](https://os.mbed.com/docs/mbed-os/latest/apis/mbed-statistics.html)
* [Mbed OS 설정](https://os.mbed.com/docs/mbed-os/latest/reference/configuration.html)
* [Mbed OS 시리얼 통신](https://os.mbed.com/docs/mbed-os/latest/apis/serial-communication.html)
* [Mbed OS 베어메탈](https://os.mbed.com/docs/mbed-os/latest/reference/mbed-os-bare-metal.html)
* [Mbed 보드](https://os.mbed.com/platforms/)

## 라이선스 및 기여

이 소프트웨어는 [Apache-2.0 라이선스](LICENSE)하에 제공됩니다. 이 프로젝트에 대한 기여는 동일한 라이선스 하에 받아들여집니다.

자세한 내용은 [contributing.md](CONTRIBUTING.md)를 참조하세요.

이 프로젝트는 다른 프로젝트의 코드를 포함하고 있습니다. 원본 라이센스 텍스트는 해당 소스 파일에 포함되어 있으며, [라이선스 가이드](https://os.mbed.com/docs/mbed-os/latest/contributing/license.html)를 준수해야 합니다.
