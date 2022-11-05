# Safe-Robber-Game

1. 설명

2021년 2학기 KMU SW 소프트웨어프로젝트2 AD프로젝트


2. 팀원

|학번|이름|
|--------|---|
|20213102|황수민|
|20213360|김혜은|
</br>
🚀 코드위치 </br>

- 코드는 src 폴더 안에
- 코드 설명 문서는 documents 폴더 안에 있습니다.

</br></br>
# 🔔 프로그램 설명

코드를 실행하면 아래 사진처럼 게임 시작 창이 뜹니다. </br>
이 창에서 게임에 대한 '설명'을 보고, '플레이어 정보'와 '게임 난이도'를 설정해 게임을 시작합니다. 
</br></br>
<img src="https://user-images.githubusercontent.com/84231143/199906532-a4dfb470-4e98-43cb-b6f9-b01cc0cd2229.JPG" width="60%"> </br>

</br></br></br>
## 🌱 EASY
난이도를 [easy]로 선택한 경우, 버튼을 누르는 횟수가 힌트로 주어집니다. </br></br>
<img src="https://user-images.githubusercontent.com/84231143/199906588-0ce9c792-6c45-4592-8b68-17b411941c40.JPG" width="20%"> </br></br></br>
화면 중앙의 다이얼 버튼을 마우스로 이동시키면, 정답에 근접할수록 소리가 커지는데, 이때, 소리가 가장 큰 틱을 골라 [next] 버튼을 누르면, 상단에 현재 입력된 값이 바뀌는 것을 볼 수 있습니다. </br></br>
<img src="https://user-images.githubusercontent.com/84231143/199906618-fe0b9203-069a-4f45-b8eb-6ca1c7f8d477.JPG" width="30%">
<img src="https://user-images.githubusercontent.com/84231143/199906752-d3c2e49d-594b-4df4-a113-18a69921a18c.JPG" width="30%">
<img src="https://user-images.githubusercontent.com/84231143/199906763-5e6afc68-e8bb-4eb1-a023-6a0f6080ae1f.JPG" width="30%"> </br></br>

기록판의 각 자리 숫자가 끝까지 바뀌였을 때, 게임이 종료됩니다. </br>
정답을 맞췄다면, 게임 랭크와 게임을 플레이하는데 걸린 시간이 같이 출력됩니다. 게임 순위는 정답을 맞춘 사람들 중 가장 시간이 적게 걸린 순으로 등수가 정해집니다. </br>
종료를 누르면, 내 기록을 저장할 것인지 물어보는 창이 뜹니다. 이때, [ok]를 누르면 저장되고, [cancle]을 누르면 저장되지 않고 종료됩니다. </br></br>
<img src="https://user-images.githubusercontent.com/84231143/199906775-c22b48f2-437a-4ec6-aad4-f64d93a57368.JPG" width="20%">
<img src="https://user-images.githubusercontent.com/84231143/199906779-37ae0222-77f9-4783-8910-7d26e6af0e78.JPG" width="20%">

</br></br>
정답과 일치하지 않으면, 개임랭크와 내가 추측한 답, 정답을 모두 보여줍니다.</br> 게임에 실패했을 시, 이때 플레이 시간은 출력되지 않고, 저장 버튼도 없습니다. 그대로 게임 끝입니다.
</br></br>
<img src="https://user-images.githubusercontent.com/84231143/199906789-87684029-211a-4daf-83aa-a6e8409a675c.JPG"  width="20%"> </br>

</br></br></br>
## 🎃 HARD
난이도를 [hard]로 선택한 경우, 버튼을 누르는 횟수가 안 주어지고, 틱의 수를 더 많이 설정해 유추하기 어렵게 만들었습니다.</br> easy와 플레이 방법이 동일합니다. </br></br>
<img src="https://user-images.githubusercontent.com/84231143/199906734-d924ac52-d034-4325-becc-a2f905541d60.JPG" width="60%"> </br>
<img src="https://user-images.githubusercontent.com/84231143/199906740-cfe54eba-bff5-46df-8def-3b031a9ce7d9.JPG" width="20%"> 
<img src="https://user-images.githubusercontent.com/84231143/199906653-d09406c9-1bf1-47a4-aa42-2145c1624848.JPG" width="20%">
<img src="https://user-images.githubusercontent.com/84231143/199906683-cb5de299-1fe9-47eb-b77c-27d103921748.JPG" width="20%">
<img src="https://user-images.githubusercontent.com/84231143/199906710-e66f1b70-5039-40b9-8c60-24f234f9f723.JPG" width="20%">

</br></br></br>
⚡랭킹을 저장할 파일은 easy, hard 난이도 각각 따로 만들었습니다. </br>

</br></br></br>
## 🤝 파트 분배
commit 및 활동 기록 상세 내역입니다. (빠진 내용이 많아 대략 이렇게 했다는 참고용으로 봐주세요)

</br>
황수민 : 화면 동작 코드 구현, 코드 및 문서 전체 점검 </br>
김혜은 : 아이디어, 화면 UI 구현, 문서작성, 발표 </br>


</br></br>
**황수민**
- 사운드 모듈 winsound에서 QSoundEffect로 교체
- 랭킹 저장 시에 데이터가 중복저장되던 오류 수정
- beep.wav 파일 추가 (틱 움직일때 출력할 효과음)
- 프로그램 아이콘 추가
- 난이도가 hard일 때, 다이얼 범위를 1~40으로 수정
- 정답 리스트에 담긴 숫자 셔플하기
- 게임에 대한 설명을 user_info.py에 추가하기
- 다른창에도 프로그램 아이콘 반영하기
- 페이지 안 끝났는데, 6자리 될 때, 게임 실패로 처리하기
- next, ok 버튼 이름 상황에 따라 바뀌도록 설정
- 난이도 설명 수정
- 유저 정보 입력 창에 게임 설명 추가
- 난이도가 'Easy'일 때도 버튼 횟수가 뜨지 않던 오류 수정
- 숫자가 6자리가 넘어가도 계속 진행되던 오류 수정
- 랭킹 표시가 이름 기준으로 되던 오류 수정
- 결과 창에 내가 쓴 비밀번호와 정답을 표시하도록 추가
- 게임 실패 시 사이렌 소리 추가
- 코드 전체점검 (변수명 정리, 파일간 연결 오류 해결)
- 문서 전체 점검 (구조설계서, 상세설계서)
- 발표 ppt 만들기

</br></br>
**김혜은**
- play_sound() 구현
- easy_explain, hard_explain 라벨 추가
- 난이도가 Easy 일 때 버튼을 누르는 횟수를 알려주는 QLineEdit() 추가
- 난이도 설명을 유저정보 입력창에 추가
- 난이도 '쉬움'일 때, 게임창에 page에 대한 정보 제공.
- 필요없는 레이아웃 삭제, GUI 코드 순서 통일성 있게 수정
- play_beep_sound 메소드 코드 가독성 있게 수정.
- 요구사항 명세서 문서작성
- 소프트웨어 구조 설계서 및 상세 설계서 작성
- README.md 작성
- 실행 영상 촬영
