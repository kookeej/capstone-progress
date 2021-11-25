2022년도 캡스톤디자인 Progress👨‍💻
===
2022년도 캡스톤디자인 Progress 기록✍

## 주차별 Progress 기록(2021년 2학기)
### 1주차(📆10/1~10/6)
> #### 교수님 코멘트
> 데이터 수집/활용 계획 구체화, 공부한 내용을 어떻게 활용할 것인지
* `국희진`: Flask 가상환경 생성 방법, Flask서버-라즈베리 파이 연동 및 코드 분석, 이미지 데이터셋(고라니, 멧돼지) 모으기 위한 웹 크롤러 수정, 적절한 사람 이미지 데이터셋 검토 중.
* `박재현`: Flask 기본적 개념, 환경세팅, 기본 예제 공부 ([`Flask 클론코딩`](https://www.youtube.com/channel/UCCaunu3Cv09ZCDxU13Gx3Hg/videos), [`Flask 기초설명`](https://wings2pc.tistory.com/entry/%EC%9B%B9-%EC%95%B1%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D-%ED%8C%8C%EC%9D%B4%EC%8D%AC-%ED%94%8C%EB%9D%BC%EC%8A%A4%ED%81%ACPython-Flask-%EC%84%A4%EC%B9%98-%EB%B0%8F-%EC%9B%B9-%EC%95%A0%ED%94%8C%EB%A6%AC%EC%BC%80%EC%9D%B4%EC%85%98Web-Application-%EC%8B%9C%EC%9E%91))  
기존 저장되어있는 영상을 인식하는게 아닌 스트리밍중인 영상의 실시간 객체인식이 필요하기 때문 추가 공부가 필요할 것.


  스트리밍 영상 객체 인식 구현 방향
  1. 실시간으로 스트리밍 중인 영상 로드  
  2. 영상속 객체를 yolo를 통해 인식  
  3. 인식되었을 때 사진을 캡처하여 저장


  다음 목표 : 파이카메라를 통해 얻은 실시간 영상을 감시하여 지속적인 객체 인식이 가능하게 하는 것.  
* `송혜민`: 우선 https://youtube.com/playlist?list=PLmEhRs1HB7REpPG4vejEgmQpLNCMC0XkB 해당 유튜브에서 다트 언어의 기본적인 변수들을 공부하였다. 영상 자체는 정말 기초적인 것들을 알려주고있기 때문에 어플 개발을 위해선 교재를 이용하여 추가로 예제연습등을 해보는편이 도움이 된다고 생각한다.
 생각해두고 있는 교재는 [오후두시]오준석의 플러터 생존코딩 책. 좀 더 알아보고 예제가 많은 책으로 구매하여 공부할 예정


* `이경로`: 플라스크 서버에 대한 지식이 하나도 없기 때문에, 일단 먼저 플라스크 공부를 시작했다. 웹 페이지는 알겠는데, 웹 서버는 그 데이터를 어떻게 저장하는 것인지? 그렇다면 구축한 서버와 라즈베리파이, 어플 간 통신은 어떻게 하는 것인지?
[`flask + rpi`](https://www.youtube.com/watch?v=RPqSbdce5EM&ab_channel=ODIY%ED%95%9C%EA%B5%AD%EA%B3%BC%ED%95%99%EC%B0%BD%EC%9D%98%EC%9E%AC%EB%8B%A8)
라즈베리 파이에 대한 정보도 잘 모르겠어서, 셋업부터 새로 공부하고 있다.
[`setup 1`](https://www.youtube.com/watch?v=tenLLerqop8&ab_channel=%EA%B3%B5%EB%8C%80%EC%84%A0%EB%B0%B0)
[`setup 2`](https://www.youtube.com/watch?v=_LB6z7e0kIE&ab_channel=%EA%B3%B5%EB%8C%80%EC%84%A0%EB%B0%B0)
[`blog`](https://seolin.tistory.com/99)



### 2주차(📆10/7~10/13)
> #### 교수님 코멘트
> 데이터셋은 실제 CCTV와 비슷한 이미지로 수집할 것. 데이터의 양보다는 퀄리티가 중요.
> 공부한 내용 프로젝트에 어떻게 적용하는지 발표
* `국희진`:-구축한 서버에 다른 네트워크로 접속이 가능한지 실험 -> LTE로는 접속 불가능&다른 와이파이로는 접속 무한 로딩. -OpenCV를 활용하여 파이카메라 제어하는 법 공부. -기존 지능형 CCTV는
어떤 통신 방법을 쓰는지 조사.
* `박재현`: 2주차의 목표를 달성하기 위해 영상을 감시하여 객체를 감지하여 영상으로 송출하는 실습을 진행하였다. 웹캠과 동영상 모두 객체 인식에 성공했고, 터미널 창에서 영상 출력까지 진행 되었다. 실제 프로젝트에서는 객체가 인식될 때 사진을 캡처해 저장 해야하므로 3주차 목표를 웹캠에 감지된 물체를 캡처하는 것으로 목표를 설정할 것이다.
* `송혜민`:
* `이경로`: CCTV에 찍히는 고라니 사진을 찾기가 어렵다. 일단 되는 대로 모아보고 이 사진을 흑백으로 처리해서 사용해야 할 것 같다. 고라니가 사슴과 노루와 비슷하게 생겨서, 사슴 | 노루 사진을 찾아보는 것도 고려하고 있다.

### 3주차(📆10/14~10/20)
> #### 교수님 코멘트
* `국희진`: 사람 데이터셋 정리
* `박재현`: 웹캠을 실시간으로 감시하여 인식되는 객체를 캡처하여 저장할 수 있도록 할것.
* `송혜민`:
* `이경로`: [플라스크 웹사이트 클론코딩](https://www.youtube.com/playlist?list=PLqIc89sXpwUBmr0Z282fm9JurDDYBE55r) 강의를 모두 수강했음. 많은 내용이 담겨 있진 않아서 현재 [Do it! 점프 투 플라스크](https://wikidocs.net/book/4542)로 공부하는 중.


### 4주차(📆10/21~10/27)
> #### 교수님 코멘트
> 시스템 구성도 좀 더 보완하기    
> 프레임 단위로 사진이 캡쳐되는 문제는 '샘플링'기법을 사용하면 문제 해결에 도움이 될 것
> 개발 환경 구축에 시간을 많이 투자해서 제대로 구축할 것
* `국희진`: -라즈베리파이 os설치, 필요 패키지/라이브러리 설치, 개발환경(vscode연동, vns, 스트리밍 웹 서버)구축. -flutter 애뮬레이터까지.
* `박재현`: 
* `송혜민`:
* `이경로`:

### 5주차(📆10/28~11/3)
> #### 교수님 코멘트
> 야생동물 데이터로 객체 인식 실험 가장 우선적으로 진행하기
> 최대한 객체인식이 시각적으로 보여지는 스트리밍 영상을 서버에 송출할 수 있도록 하기.
* `국희진`: -Flutter json 데이터 송수신. -라즈베리파이 환경 세팅.
* `박재현`: 경로와 함께 라즈베리파이 원격 접속후 파이카메라를 스트리밍에 성공하였다.  
 **다음 목표인 파이카메라의 영상 로드 후 객체 인식**을 위해 영상을 가져오기 위한 방법이 필요 했고, 
 웹스트리밍 예제코드를 참조했던 사이트에서 참고가 가능하였다. [**`웹 스트리밍을 Opencv를 통해 가져오기`**](https://webnautes.tistory.com/1262)  
 
   **웹서버의 영상은 URL로 접근**이 가능했다.  
   이는 앞으로 만들 플라스크서버의 영상 또한 같은 방식으로 로드 할 수 있을 것이다.
   
   영상을 웹에서 접근하여 가져오고, 다시 객체 인식하는 과정이기 때문에 **약 3초의 지연시간이 발생하는 문제점**이 발견되었다.
 
   다음주 목표 : 객체탐지의 지연을 줄이기위해 **파이카메라에서 바로 영상을 가져오는 방식**을 공부할 것.  
   [**`파이카메라 영상의 웹 스트리밍 예시 코드`**](https://github.com/jacksonliam/mjpg-streamer) 참조.
* `송혜민`:
* `이경로`: vnc와 vscode의 ssh-remote로 라즈베리파이 원격 접속을 성공했다. [Raspberry Pi에서 mjpg-streamer를 사용하여 웹캠 스트리밍하기](https://webnautes.tistory.com/1261)에서 웹캠 스트리밍하는 방법을 시도해보았다. 딜레이는 거의 없는 것으로 확인했고, 객체 인식은 파이에서 직접할지, 서버로 넘긴 후 처리할지 고민해봐야 할 것 같다. `주의점`은 **vnc로 화면을 연 상태로 ssh를 실행해야 제대로 작동한다. ~~또한 내 노트북(macOS)로는 되지 않았고,~~ macOS, Windows에서도 실행 가능하게 되었다.**
* `이경로`: 우리 카메라 모듈은 [라즈베리 파이 NOIR 5MP OV5647](https://www.devicemart.co.kr/goods/view?no=12232529)인데, 적외선 카메라가 되는지는 아직 잘 모르겠다. 인터넷을 찾아보니 연결하면 바로 이용이 가능하다고 했는데 저조도에서 적외선 영상이 촬영되지 않았다.

### 6주차(📆11/4~11/10)
> #### 교수님 코멘트
* `국희진`: -라즈베리파이 서버, 외부(pc)서버 분리. 라즈베리파이 서버는 카메라 영상만 전송하고 외부(pc)서버는 영상을 받아 웹에서 스트리밍.
* `박재현`: 
* `송혜민`:
* `이경로`:

### 7주차(📆11/11~11/17)
> #### 교수님 코멘트
> * recall에 좀 더 무게를 둬도 좋을 것. 
> * 탐지된 객체 표시할 때 바운딩 박스 외에 퍼센티지도 함께 표시하면 실패에 대한 대비책으로 내세울 수 있을 것
> * 하지만 최대한 성능 개선에 집중할 것
* `국희진`: 바운딩 박스가 표시된 영상을 웹스트리밍으로 확인할 수 있도록 함. 객체 탐지될 때 서버에 신호주기.(True/False)
* `박재현`: 
* `송혜민`:
* `이경로`:

### 8주차(📆11/18~11/24)
> #### 교수님 코멘트
* `국희진`: 서버와 파이어베이스 연동. 객체 탐지 정보(탐지 여부, 탐지 시간) 파이어베이스 real-time database로 
* `박재현`: 
* `송혜민`:
* `이경로`:
