# final-pjt

1️⃣ 팀원 정보 및 업무 분담 내역

윤동훈 : 기획, front, back, 데이터베이스 모델링, 발표
설혜현 : 기획, front, PPT
2️⃣ 목표 서비스 구현 및 실제 구현 정도

목표 서비스 : 실시간 한줄평을 통해 유저들의 다양한 의견을 공유
실제 구현 정도 : 각 영화에 대한 리뷰 게시판을 통해 다양한 의견을 공유 가능하게 함.
목표 서비스 : 좋아요 누른 영화 데이터 기반으로 새로운 영화 추천 알고리즘
실제 구현 정도 :

좋아요 한 영화의 장르를 기반으로 새로운 영화 추천
회원가입 후 최초 로그인 회원은 데이터가 없기 때문에 랜덤으로 영화 추천
좋아요가 3개 미만인 경우, 좋아요 한 영화의 장르 중 선택된 횟수가 가장 많은 하나의 장르에서 평점순으로 추천
좋아요가 3개 이상인 경우
장르 3가지가 모두 포함되는 영화 추천
장르 중 2가지가 포함되는 영화 추천
개수가 많은 장르 1가지인 영화 10개 추천
3️⃣ 데이터베이스 모델링 (ERD) ERD 4️⃣ 영화 추천 알고리즘에 대한 기술적 설명 (/uploads/f7df3a86489d8580f9caf82856418a3a/Final_PJT_알고리즘_순서도.drawio.png) 5️⃣ 서비스 대표 기능에 대한 설명 < 한줄평 > 실제 사용자가 남긴 리뷰 중 한줄평 부분만 추출해, 평점과 함께 movie detail page에 게시 < 영화 추천 알고리즘 > - 좋아요 한 영화의 장르를 기반으로 새로운 영화 추천 - 회원가입 후 최초 로그인 회원은 데이터가 없기 때문에 랜덤으로 영화 추천 - 좋아요가 3개 미만인 경우, 좋아요 한 영화의 장르 중 선택된 횟수가 가장 많은 하나의 장르에서 평점순으로 추천 - 좋아요가 3개 이상인 경우 1. 장르 3가지가 모두 포함되는 영화 추천 2. 장르 중 2가지가 포함되는 영화 추천 3. 개수가 많은 장르 1가지인 영화 10개 추천 6️⃣ 배포 서버 URL X 7️⃣ 기타 (느낀점,후기 등) 한 학기동안 배운 것들을 활용하여 직접 프로젝트를 진행 해 보니 많은 도움이 되었다. 수업시간에는 이해되지 않은 것들이 있었는데 실제로 기능을 구현해보면서 이해가 된 것들도 있었다. 앞으로 2학기 때 진행될 프로젝트들을 위해 더 많은 공부를 해야겠다고 느꼈다.

:memo: 0518 Project Record
:seedling: Ready

Moviecard 레이아웃
Now playing, Upcoming 클릭 > Moviecard로 이동
django 데이터 넣기
Search > 검색 > 검색어와 관련된 영화 보여주기
Search > 검색 > 검색 해당 단어와 관련된 모든 영화 보여주기
:potted_plant: In Progress :deciduous_tree: Done

Moviecard 레이아웃
Now playing, Upcoming 클릭 > Moviecard로 이동
django 데이터 넣기
Search > 검색 > 검색어와 관련된 영화 보여주기
Search > 검색 > 검색 해당 단어와 관련된 모든 영화 보여주기
:exploding_head: error

Homeview > Upcoming, Now playing 클릭하면 Moviecard페이지로 넘어가도록 구현 :no_entry:️ 새로고침 시 데이터가 초기화 됨
해결방법 : 포스터 클릭 시 해당 영화 id를 가지고 다시 tmdb에서 axios로 영화 데이터 받아오기

:memo: 0519 Project Record
:seedling: Ready

Moviecard 디자인
Moviecard 카드 올라가는 느낌으로 구현
데이터 '영화ID'까지 들어있도록 다시 받아오기
리뷰 댓글 창 토글로 숨기기 기능
Show More 클릭 > Movie Top10 detail page로 전환
article 구현
:potted_plant: In Progress

Moviecard 카드 올라가는 느낌으로 구현
:deciduous_tree: Done

Search button 클릭 > Moviecard로 전환
데이터 '영화ID'까지 들어있도록 다시 받아오기
article 구현
Show More 클릭 > Movie Top10 detail page로 전환

:memo: 0520 Project Record
:seedling: Ready

User 페이지 구현
프로필 페이지
Show More 클릭 > Movie Top10 detail page로 전환
Top10 카드형식으로 각각 영화 정보 component 담아서 불러오기
:potted_plant: In Progress

:star2:알고리즘 추천 기능 더 자세히 생각해서 틀 구현
전체적인 디자인 detail 수정
:deciduous_tree: Done

User 페이지 구현
프로필 페이지
Show More 클릭 > Movie Top10 detail page로 전환

:memo: 0521 Project Record
:seedling: Ready

로그인& 로그아웃
Review page 디자인
back 기본기능 다 구현
user 토큰 가져와서 글 작성할 때 이름 불러오기
로그인 하지 않은 user click 막고, login modal 보여주기
좋아요,리뷰 보러가기 버튼 구현
프로필 페이지 완성
:potted_plant: In Progress

:star2:알고리즘 추천 기능 더 자세히 생각해서 틀 구현
전체적인 디자인 detail 수정
좋아요,리뷰 보러가기 버튼 구현
Review page 디자인
프로필 페이지 완성
:deciduous_tree: Done -back 기본기능 다 구현 -로그인& 로그아웃 modal

user 토큰 가져와서 글 작성할 때 이름 불러오기
로그인 하지 않은 user click 막고, login modal 보여주기

:memo: 0522 Project Record
:seedling: Ready

:star2:알고리즘 추천 기능 더 자세히 생각해서 틀 구현
프로필 페이지 완성
좋아요,리뷰 보러가기 버튼 구현
MovieCard 완성
:potted_plant: In Progress

:star2:알고리즘 추천 기능 더 자세히 생각해서 틀 구현
전체적인 디자인 detail 수정
Review page 디자인
MovieCard 완성
:deciduous_tree: Done

프로필 페이지 완성
좋아요,리뷰 보러가기 버튼 구현
검색 했을 때 movieCard 페이지로 연결

:memo: 0523 Project Record
:seedling: Ready

좋아요 버튼 구현
프로필에 나온 포스터 영화 클릭 시 디테일 창과 연결
MovieCard 댓글창 구현
MovieCard 완성
리뷰페이지 좋아요 버튼 구현
프로필페이지 리뷰 댓글 detail
한줄평 없을 때 에러 제거
HomeView에서 영화 포스터 boder 등 디테일 주기
프로필페이지 글자 정렬
MovieCard에서 리뷰작성 할 때, modal창 디자인
MovieCard overview 글자 정렬
:potted_plant: In Progress

:star2:알고리즘 추천 기능 더 자세히 생각해서 틀 구현
전체적인 디자인 detail 수정
MovieCard 완성--->왼쪽정렬
프로필페이지-->comment 창
리뷰페이지 좋아요 버튼 구현
프로필에 나온 포스터 영화 클릭 시 디테일 창과 연결
:deciduous_tree: Done

MovieCard 댓글창 구현
MovieCard 완성
좋아요 버튼 구현
프로필페이지 글자 정렬
프로필페이지 리뷰 댓글 detail
MovieCard에서 리뷰작성 할 때, modal창 디자인
HomeView에서 영화 포스터 boder 등 디테일 주기
MovieCard overview 글자 정렬

:memo: 0524 Project Record
:seedling: Ready -알고리즘 마무리

Recommend 페이지 완성
프로필 사진 다 바꾸기
리뷰list 좋아요 버튼 구현
전체적인 디자인 detail 수정
:potted_plant: In Progress

:star2:알고리즘 추천 기능 더 자세히 생각해서 틀 구현
전체적인 디자인 detail 수정
MovieCard에서 리뷰작성 할 때, modal창 디자인---> 코드 합ㅊㅣ기
리뷰페이지 좋아요 버튼 구현
프로필에 나온 포스터 영화 클릭 시 디테일 창과 연결
리뷰list 좋아요 버튼 구현--> 새로고침 후에도 변하지 않도록
:deciduous_tree: Done -알고리즘 마무리

Recommend 페이지 완성
프로필 사진 다 바꾸기
리뷰list 좋아요 버튼 구현
전체적인 디자인 detail 수정

:memo: 0525 Project Record
:seedling: Ready

알고리즘 마무리
발표 자료 준비
detail한 부분 디자인 수정(글꼴, 정렬, 404페이지)
댓글 및 리뷰 예시 작성
로고 디자인
:potted_plant: In Progress

:star2:알고리즘 추천 기능 더 자세히 생각해서 틀 구현
전체적인 디자인 detail 수정
MovieCard에서 리뷰작성 할 때, modal창 디자인
리뷰페이지 좋아요 버튼 구현
리뷰list 좋아요 버튼 구현--> 새로고침 후에도 변하지 않도록
댓글 실시간 업로드
:deciduous_tree: Done

알고리즘 마무리
발표 자료 준비
detail한 부분 디자인 수정(글꼴, 정렬, 404페이지)
댓글 및 리뷰 예시 작성
로고 디자인
리뷰페이지 좋아요 버튼 구현
MovieCard에서 리뷰작성 할 때, modal창 디자인
댓글 실시간 업로드