# 버전 0.1 ~
## 개요
웨이트 트레이닝을 하면서 운동한 내용을 무게, 횟수, 세트수, 쉬는시간(Optional) 등을 기록하고, 사이클을 돌아 다시 운동할 때 이전의 데이터를 보기좋게 정리하여 보여줘서 점진적 과부하를 달성하기 수월하도록 하고 싶습니다.
최초 목적은 운동 기록을 작성하는 것에서 기회가 된다면 근육 부위별 운동 정보를 보여주어 운동할 때마다 찾아서 하는게 아니라 한 페이지 내에서 정리된 운동정보를 보고 싶어서 웹페이지 제작을 시작했습니다.

## 사용한 기술
* 언어 : HTML / CSS / Javascript

## 동작
▶ 버전 0.1 : 메인 페이지를 만들고 메인페이지에서 운동정보, 운동기록 등으로 이동할 수 있는 링크를 추가하여 마우스 포인트 이동 시 밑줄을 그어 사용자가 링크임을 알 수 있게 하였습니다.(차 후 업데이트로 각 링크를 통해 페이지 이동이 가능하게 하고, 각 링크로 이동 시 필요한 정보를 얻거나 기록이 가능하게 하는 내용을 추가)
* 아직 구현가능한 HTML / CSS 및 Javascript 기술이 부족하여 Website를 선 제작 후 공부하며 개선해나갈 예정입니다.

▶ 버전 0.2 : 메인 페이지 하단부에 메뉴에 커서가 닿기도 전에 효과가 나타다 수정, background 이미지 align 센터로 수정.
+) Javascript, Media query를 이용하여 550px 미만일 때 아래 메뉴가 사라지고, bar 버튼을 통해 상단에 메뉴가 나타나게 추가하였습니다.

▶ 버전 0.3 : bar 버튼으로 생성된 메뉴들에 커서 위치 시 background-color 변경 → color 변경 및 transition 추가하여 자연스럽게 변경, 사진 용량 Down
 * Workout Information 창 추가하여 Concept 작성, 세부적인 내용 및 Design은 변경 예정.
 * 버전 0.3.1 : Workout Information 창에 사진 및 사진에 hover 시 div transform을 통해 아래쪽에서 클릭 가능한 창 올라오고, 글자에 따로 hover 시 색깔 변화를 줘서 클릭 가능한지 구분 가능하게 변경.
 * 버전 0.3.2 : 사진에 hover로 나타나는 글씨를 클릭하면 해당 운동 정보가 나타나는 popup 창 추가하였습니다.(해당 버전에선 운동 1개만 적용 중)
 * 버전 0.3.3 : 각 사진에 해당하는 운동 정보를 추가하였고, 화면 좌측에 sideBar 를 추가하여 추후 해당 부위별 운동 정보를 사용자가 쉽게 접근할 수 있도록 만들었습니다.
 * 버전 0.3.4 : PC 화면으로 보면 의도한대로 나오지만, 일정 PX 미만의 Mobile 등으로 확인하면 사진이 잘리고 sideBar도 잘려 일정 PX 미만일 때 sideBar를 Toggle 버튼을 만들어 없애고 나타날 수 있게 수정하였고, 운동정보 확인할 때 화면이 잘려 JS를 이용해 일정 PX 미만일 때 크기가 알맞게 줄어들도록 수정하였습니다.
 * 버전 0.3.5 : 현재 화면이 어떤 화면인지 알 수 없어 현재 페이지를 중앙부에 표시하였고, 화면이 작아졌을 때 나타나는 bar icon이 직관적이지 않아 아래, 위 화살표를 삽입하여 화살표 클릭 시 toggle 메뉴가 나오고, bar 클릭 시 main link가 나오도록 수정하였습니다.
 * 버전 0.4 : 화면이 일정 px 이상일 때 main link는 항상 표시되도록 수정하였고, 넓을 때도 현재 페이지를 색깔로 표시하여 사용자가 인식 가능하게 함. +) JS를 이용해 운동 분류 tap click 시 title을 바뀌게하여 사용자가 현재 페이지를 인식할 수 있게 함.

▶ 버전 0.4 : Workout Log Page 추가. 최초 아이디어로 이전 운동 기록 확인 링크와 운동 기록 입력 링크 두가지로 나뉘어 표시함. 직관적으로 알아볼 수 있는 아이콘 이미지를 활용하였고, 이미지에 커서 이동 시 link 이동 정보를 translate 하여 보여줌.
 * 버전 0.4.1 : Workout Log Page에서 당일 운동 계획 메뉴를 추가하였고, 해당 메뉴는 차후 진입 시 당일 날짜, 시간 등이 표시되고, 해야할 운동의 종목을 입력하여 버튼을 클릭하면 List가 형성되어 Check 또는 Delete가 가능하도록 추가할 예정.
 * 버전 0.4.2 : 당일 운동 계획 메뉴에 들어가면 Date 객체를 이용해 접속했을 때의 날짜, 요일, 시간 등을 표현했고, 아래 Text 타입 input을 추가하여 사용자가 운동 계획을 추가할 수 있도록 하였음.
 * 버전 0.4.3 : Input에 값을 입력하면 Input 창 아래에 입력한 list가 나오게 되고, check 버튼, delete 버튼을 추가해서 check 버튼 클릭하면 line through가 되어 사용자가 check한 것을 눈으로 인식할 수 있게 하고, delete 버튼을 누르면 transform 후 지워지는 애니메이션을 추가 / filter 할 수 있는 select를 추가.(아직 기능은 미구현)
 * 버전 0.4.3.1 : filter 기능을 수행하는 select를 추가하여 complete 시 check 되어있는 list만 보여주고, uncomplete 시 check가 되어있는 list를 제외한 나머지 list들을 보여주도록 추가.
 * 버전 0.4.3.2 : Workout Log 창 들어갔을 때 나타나는 아이콘 3개의 배경색을 파스텔 톤으로 변경해서 보기 편안하게 수정.
+)Workout Log 창에서 Select를 추가하여 가슴~팔 등 5가지의 분할을 선택할 수 있게했고, 선택함에 따라 나타나는 radio type input에 따라 클릭하면 자동으로 input text 칸에 입력되도록 수정(현재 radio 체크박스는 가슴 운동만 표시되며 기능 추가 예정)
 * 버전 0.4.3.3 : Set 수, 무게(kg)을 간단하게 설정할 수 있는 Select를 만들었고, 해당 Select를 설정하면 Input Text값에 자동으로 입력되게 기능 추가함, 초기화 버튼을 생성하여 입력한 내용을 모두 지울 수 있도록 설정, CSS를 수정해서 좀 더 보기 좋은 색상, 모양으로 변경.

▶ 버전 0.5 : 최초 홈페이지 접속 시 이동 가능했던 메뉴 중 main page 추가. 해당 페이지에서는 Fitness Manager에서 제공할 수 있는 정보를 한눈에 볼 수 있도록 근성장의 3요소를 사진과 함께 추가하여 사용자가 직관적으로 이해할 수 있게 했고, CSS를 이용해 사진을 클릭하기 전에 Transform 효과를 추가함.
 * 버전 0.5.1 : 오늘 운동 계획 페이지에서 "운동 종목 선택" 셀렉트를 선택하면 해당 부위에 맞는 대표 운동 6가지가 나타나게 하고, 다른 부위 선택 시 해당 부위만 표시되도록 기능 추가.
main 페이지에서 그림에 나타나는 글씨가 작아 크기 수정.

### Source code
###### 메인 : https://junhyeong-b.github.io/fitmanager.html
###### FITNESS MANAGER : https://github.com/Junhyeong-B/Junhyeong-B.github.io/blob/main/fitmanager.html
###### Workout Information : https://github.com/Junhyeong-B/Junhyeong-B.github.io/blob/main/workoutinfo.html
###### Workout Log : https://github.com/Junhyeong-B/Junhyeong-B.github.io/blob/main/workoutlog.html
###### Workout Log - Today workout List : https://github.com/Junhyeong-B/Junhyeong-B.github.io/blob/main/logtodo.html
###### Main : https://github.com/Junhyeong-B/Junhyeong-B.github.io/blob/main/main.html
