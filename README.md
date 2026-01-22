Chapter 6. 인터페이스 설계하기

# 와이어프레임에 빠르게 아이콘 넣기 위한 iconify 플러그인
1) community -> icon 검색 -> plugin -> iconify 플러그인 설치
2) 와이어프레임 page -> 플러그인 -> iconify 패널 띄움 - 검색
   - 아이콘은 벡터 형태로 저장됨
   - [back]은 [<] chevron
3) 아이콘 선택 및 customize icon -> parent layer and alignment (패널 하단에 어느 frame, 상하좌우/센터 어느 위치에 불러올지 설정) -> drag&drop or 불러올 위치 select해두고 [import icon] 클릭

# Auto Layout의 개념 이해하기
Auto Layout(이하 AL) : 여러 형태의 UI 요소가 있고, 웹/모바일과 변동되는 요소들에 상관없이 동일한 레이아웃으로 사용하기 위해 설정하는 기능
1) 요소들 select -> AL 패널에 [+] -> Layers 패널에 해당 요소들 묶여있고 AL 표시되어있음.
2) AL 패널에서 정렬 방향(수직/수평) -> 요소들끼리의 간격 -> padding(요소들과 전체 사이 margin) 설정 -> (간격 따로 설정하고 싶다면) Alignment and padding 상하좌우 따로 설정 가능 + 정렬 방향 + packed (안쪽의 요소들이 설정해둔 간격대로 순차적으로 고정된 사이즈로 들어갈 때) / space between (꽉 채워 균일한 간격으로 들어갈 때 auto 같은)

# Constraints & Resizing의 개념 이해하기
1) Constraints : frame을 기준으로 그 안 요소에 제약을 둬서 frame 사이즈 조절할 때 안쪽 요소의 위치 설정하는 기능
   - e.g. 하단+왼쪽 select = 그 밖 frame을 늘렸을 때 하단 왼쪽은 고정되고 늘어남.
2) Resizing : AL된 상태에서 상세 속성으로 지정할 수 있는 기능.
   - Container : 요소를 감싼 요소(frame). 컨테이너 대비해 안쪽 요소의 사이즈를 조정하거나 앙쪽 요소에 대비해 컨테이너 사이즈 조정하는기능.
   - padding처럼 안쪽 요소의 사이즈를 fixed width/fixed height -> fit container
   - 요소를 끌어서 순서 변경도 가능.
   - 두 개 이상이 fill이면 균등하게 분배돼서 채워짐.
   - Container resizing : 
