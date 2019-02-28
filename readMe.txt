0. git bash 다운,
0-1. 깃허브 홈페이지 로그인 후 레퍼지토리 생성
0-2. 원하는 위치에 폴더 생성
===
1. 생성한 폴더 오른쪽 클릭 후 git bash here 클릭,

2. 창이 뜨면 초기화하겠다는 의미로
	git init
   코드를 치면 생성했던 폴더 안에 .git 이라는 폴더가 생성됨.

3. 이후 생성했던 폴더를 깃허브의 레퍼지토리에 연결하기 위해
 	git remote add origin https://github.com/iooool/startGit.git
   라고 침. 이 때 git remote add origin 이후에는 내가 생성한 레퍼지토리의
   주소를 입력하면 됨. 코드를 치면 아무런 변화 없음.

4. push 전엔 pull을 기본적으로 해야함. 지정한 repository에서 모든 자료를
   한번에 끌어오기 위하여
	git pull origin master

5. 여기부터는 push 영역. 현재 나의 로컬 폴더와 git과의 싱크 상태를 
   체크하기 위해
	git status

6. 현재 나의 로컬 폴더와 git 사이에 변경된 파일이 있을 경우 모두 tracking 위해
	git add .

7. 변경사항 업로드 시 사람들에게 알려주는 커밋을 달수있음.
	git commit -m " 메시지를 입력해주세요 "

8. 실제로 git에 push를 요청함.
	git push origin +master