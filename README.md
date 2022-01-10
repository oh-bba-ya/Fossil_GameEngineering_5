# 두더지의 저주
게임공학 5조 이로운 배건우 곽명석 - (fossil 저장소에 코드 존재)

닷지와 같은 유형의 게임으로 두더지의 저주를 받은 두더지 잡기 세계 챔피언은 갑자기 두더지가 되어 고양이와 농부들로부터 도망다니며 토마토, 식물을 먹어야하는 운명이 되었다.
과연 끝까지 살아 남을 수 있을것인가..!

# 구글 드라이브
+ perforce_mole.egg 파일의 경우 프로젝트 파일입니다.
+ WindowNoEditor.zip 파일은 exe 실행 압축 파일 입니다.
https://drive.google.com/drive/u/0/folders/1U8EebdHDE7wt7C25tr1o25eT7CCHUtDQ

## 게임 조작법
+ W , A , S , D : 플레이어 이동
+ Space Bar : 구멍파기
+ Mouse left Click : 먹기


### 게임 설명
+ 생존시간이 표시됩니다. 일정시간 동안 토마토 , 작물을 먹지 못하게 된다면 게임이 종료 됩니다. 또한 추적자들에게 공격을 당할시에도 게임은 종료됩니다.
+ 구멍파기를 사용하여 고양이, 농부로부터 피할 수 있습니다. 하지만 쿨타임이 존재하므로 적절한 상황에서만 사용해야 합니다.

<img width="60%" src ="https://user-images.githubusercontent.com/49023743/121403359-c6598e00-c995-11eb-98ac-ec4e8d612509.PNG"/>

<img width="60%" src ="https://user-images.githubusercontent.com/49023743/121403373-ca85ab80-c995-11eb-921a-766b94be1cdb.PNG"/>

+ 땅속에서 적의 위치를 파악 할 수 있지만 정확한 지형은 파악하지 못합니다.

<img width="60%" src ="https://user-images.githubusercontent.com/49023743/121403810-41bb3f80-c996-11eb-95ed-8888f82f0ebd.PNG"/>

<img width="60%" src ="https://user-images.githubusercontent.com/49023743/121403813-43850300-c996-11eb-82b9-1761e143b3af.PNG"/>



+ 기존에 존재하는 구덩이에서는 쿨타임 없이 사용가능합니다.
+ 풀숲에 숨는다면 추격을 피할 수 있습니다. 하지만 모든 고양이로부터는 도망칠 수 없습니다.
+ 토마토 , 도망다니는 작물을 섭취함으로써 생존시간을 높일 수 있습니다.


### 농부
+ NavMesh를 사용했습니다.
+ Environment Query System (EQS)를 사용하여 농부의 순찰 위치가 제일 높은 점수로 이동하게 됩니다.
<img width="80%" src ="https://user-images.githubusercontent.com/49023743/121378909-8dfa8580-c97e-11eb-9430-6954e9b2081b.gif"/>


### 고양이
+ Range 추적
+ Mp4 파일이므로 클릭하면 영상이 보입니다. (밑 사진모양)
<img width="80%" src ="https://user-images.githubusercontent.com/49023743/121404234-b7bfa680-c996-11eb-9de8-c311456213f4.mp4"/>


+ NavMesh 추적
+ Percetion을 사용하여 Sight를 사용하여 고양이의 시선 추적을 사용했습니다. 
+ Mp4 파일이므로 클릭하면 영상이 보입니다. (밑 사진모양)
<img width="80%" src ="https://user-images.githubusercontent.com/49023743/121404225-b55d4c80-c996-11eb-89e7-8c2088b3b55b.mp4"/>


### Crop
+ NavMesh를 사용했습니다.
+ Perception Sight를 사용하여 일정 영역에 들어오게 된다면 Navmesh 속 랜덤 좌표로 움직이게 됩니다.
+ <img width="70%" src ="https://user-images.githubusercontent.com/49023743/121379933-740d7280-c97f-11eb-9424-3ab3bddc1d4b.gif"/>

+ Mp4 파일이므로 클릭하면 영상이 보입니다. (밑 사진모양)
<img width="70%" src ="https://user-images.githubusercontent.com/49023743/121404275-c3ab6880-c996-11eb-8440-eba55a3603c4.mp4"/>


