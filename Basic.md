# =====2018.10.24(WED)=====

## 한글 설치 방법
    sudo apt-get install ibus
    sudo apt-get install ibus-hangul
    sudo apt-get install fonts-unfonts-core

 ### 카메라는 원격으로 제어할 수 없다.(라즈베리화면을 띄워놓고 해야한다.)
 ### 집에서 쓰지 않는 이상 학교나 많은 사람들이 아이피를 사용할 경우 충돌이 되어 고정아이피를 사용하지 않는 것을 추천한다.
 ### Web에서 쌍방향으로 제어가능 (pad-computer-mobie 서로 동기화가 가능하다)
 ### 220V 전원제어 -> (Relay switch)전자석으로

# ======2018.10.25THU)=====

## drone 오픈소스와 농업용 drone에 관한 자료와 영상을 강사님께 받아왔습니다.
    1. RaspberryPI는 iptime공유기랑 잘 연결되지 않는다.(추천 제품 TPLink TL-WR940N Plus)
    2. RaspberryPI는 교육용, 테스트용이라 실제에서 쓰기에는 발열문제와 쉽게 고장나는 3. 문제점이 발생해서 쓰이지 않는다.
    4. RaspberryPI를 이용해 220V전원을 제어하려면 전자석으로 Relay switch를 쓰면된다.
    5. NodeJs는 Web server이다.(for example, google GCS, Java script engine)

### braspberryPI에서 Aux단자를 통해 소리를 재생할 경우 곰오디오를 통해서 확장자를 맞춰줘야한다.
### 라즈베리파이 카메라를 이용하여 openCV를 통해 얼굴인식이 가능하다.

### 아두이노 기초강좌 - youtube"코딩런" 참고

### Virtual Box ->가상화 환경에서 구동이 가능하다
    저장소 -> 종류 ICH6 로 변경

### Python 함수 나올 때 -> exit()

## 함수 복사할때 "i"누르고 전체 복붙
        {   :q!  
        > 저장하지 않고 나오기   
        :wq  ==저장하고 나오기
        > 하기전에 "ESC"키 누르기
         HEVC
        > 압축이 2배가 가능하다. 전송을 할 떄 압축을 2배더 하거나 화질이 2배 더 좋아지게 할 수 있다.
        H265
        > 실시간 동영상 스트리밍 서비스, 차세대 압축방식

### raspberryPi로 LED제어
### 초음파센서값 읽어오기   
### 온도와 습도센서 읽어오기


# ==========2018.10.26(FRI)==========
    tera term 프로그램
    > SSH:Secure File copy
    > file을 라즈베리파이에 손쉽게 넣을 수 있다.
    > ..  ==>상위폴더 명령어

## 리눅스에 서버만들어서 노트북-라즈베리파이 연결 with teraterm
    unzip
    > 리눅스에서 압출 풀때 명령어

## node.js문 쓰는 법

    1. 폴더이름을 node로 해서 c로컬디스크에 만들어준다.
    2. 그 폴더에 js파일을 넣어준다
    3. 컴퓨터에서 cmd를 실행한다.
    4. cd \
    5. cd node
    6. node (파일명).js
    7. 서버 링크를 받아서 인터넷에서 실행한다.

    #####################################js파일문#################################################
        // 모듈을 추출합니다.
        var http = require('http');

        // 웹 서버를 생성 및 실행합니다.
        http.createServer(function (request, response) {
        response.writeHead(200, { 'Content-Type': 'text/html' });       
        response.end('<h1>Hello World .. !</h1>');  //첫 페이지에 'Hello World..'가 보여지게 설정한다.
        }).listen(52273, function () {
        console.log('Server running at http://127.0.0.1:52273/');
        });

        ################################################################################################
