# Today I Learned

### git / terminal 명령어 정리

- git fetch : 리모트 서버로부터 저장소 정보 동기화 (원격 저장소의 최신 이력 확인 가능)
- git merge : 합치기 
- git pull (= git fetch + git merge)
- git push -u origin master : 원격에(master branch에) 올리기
  - -u : upstream
  - -f : force 
- git config -- list : 설정 해 놓은 사항들을 세세히 볼 수 있음


#### git 최신 상태로 유지하기
- git pull --rebase : 저장소의 이력을 간결하게 유지하기 위해 이 명령어를 사용
- git pull --rebase origin master 

1. 원하는 repo(A)를 fork해온다.
2. fork된 내 repo(B)에서 나의 local로 clone한다.
3. 해당 폴더로 들어가 remote가 잘 되었는지 확인한다. [git remote -v]
4. 다시 A repo로 돌아가 주소를 복사해온다.
5. upstream 원격 저장소를 추가한다. [git remote add upstream 주소]
6. upstream이 잘 추가되었는지 확인한다. [git remote -v]
7. git pull --rebase upstream master로 A repo의 수정된 파일들을 pull 해온다. 
8. 내 저장소에 동기화한다. [git push -u origin master]

----

- mkdir : 폴더 만들기
- rm : 삭제
- rm -rf : 다 밀어버리겠다
  ex) tutorial 폴더를 밀어버리겠다
  ~~~
  rm -rf /tutorial
  ~~~
- cp : 파일 복사
- mv : 파일 이동 [끝의 마침표는 해당 주소로 그 파일을 옮길꺼임 이라는 뜻] 
  mv original_file new_file_path [이동 후 경로가 현재 경로인 경우엔 .을 찍어줌]
  ex) 
  ~~~
  mv ~/data/TWL/ .
  ~~~
- ls : 숨김파일 포함 X 목록
- ls - al : 숨김파일 포함 O 목록


### 특강 - 김슬 기자님 : 데이터 분석으로 세상을 바꿀 수 있을까요?
[시빅 해킹]
#### What is Civic Hacking? 
공공문제를 해결하는 프로그램을 만들거나, 공공문제를 이야기하는 프로그램을 만드는 것 

*projects*
- EXIF : 사진이나 영상 파일에 들어있는 메타 정보 
- twitter streaming api : 조금의 트윗들을 읽어올 수 있게 해주는 api (다 긁어오려면 돈내야함)
- DBSCAN
- 존맛국회 : 차이나프로..ㅎㅎㅎ.. 가보고싶다.. ㅎㅎ.. 

*open source*
- 온라인에 올라와있는 무료로 쓸 수 있는 소스들. 사람들이 "무료"에 집중하는데, "무료"보다는 "협업"을 함께 하자는 뜻으로 받아들이면 좋겠다.

#### 책 추천
- 어쩌다보니 통계학자
- 신호와 소음
- 통계학의 피카소는 누구인가
- 성당과 시장




