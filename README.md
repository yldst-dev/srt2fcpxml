# srt2fcpxml
srt2fcpxml은 srt 자막을 파이널컷 프로의 자막으로 변경해주는 유용한 도구입니다.

이 도구는 파이널컷 프로 최신 버전(10.8.1)에서 최종 테스트가 완료되었습니다.


## 최신 릴리즈 다운로드
Users who do not want to compile can download the [executable file](https://github.com/GanymedeNil/srt2fcpxml/releases) directly.

## 사용 방법
터미널을 사용해 해당 실행파일에 권한을 부여합니다. `chmod +x ./srt2fcpxml`

아래는 명령줄 도구에 사용될 인자들입니다.

```bash
$ ./srt2fcpxml
  -fd [정수]
    	영상의 프레임레이트는 아래와 같이 지원됩니다.
      23.98、24、25、29.97、30、50、59.94、60 (기본값은 25프레임 입니다.)
  -srt [경로]
    	변환할 srt 자막 파일의 경로를 입력합니다.
  -width [정수]
        가로 해상도를 결정합니다. (기본값 1920)
  -height [정수]
        세로 해상도를 결정합니다. (기본값 1080)
```

## 최종 예시

```bash
$ ./srt2fcpxml -srt /tmp/test.srt
```
위의 명령어를 입력하면 `fcpxml` 확장자를 가진 파일이 생성됩니다. 이 파일을 더블클릭하여 파이널컷 프로에서 불러오기 하면 됩니다.
