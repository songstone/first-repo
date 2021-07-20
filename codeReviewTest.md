## Git과 Github으로 Code Review 하는 법 정리

1. iterm을 이용해 해당 repo가 있는 디렉토리로 이동한다.
2. `git branch (새 branch 이름)` 명령을 이용해 새로운 branch를 만든다.
3. `git branch` 명령을 통해 현재 선택된 branch를 확인한다.(녹색으로 표시 되어있음)
4. `git switch (branch 이름)`을 통해 새로 만든 branch로 바꾸고 다시 한번 `git branch` 를 이용해 바뀌었는지 확인한다.
5. `touch (새 파일 이름)` 명령을 통해 새로운 파일을 생성한다.
6. 파일을 vi로 열어 작성하고 저장 후에 `git status` 로 확인을 한다.
7. 별 이상이 없다면  `git add (파일 이름)` 을 입력하여 변경 사항을 스테이지로 올린다.
8. `git status` 명령을 통해 잘 올라갔음을 확인 한 후 `git commit` 명령을 통해 prefix를 작성한다.
	- docs : 문서 관련
	- feat : 기능 개발 관련
	- fix : 버그 픽스 관련
	- refactor, conf, test, ...
9. 저장 후 `git status` 명령을 통해 상태를 체크 하고 별 이상이 없다면 `git push -u origin (만든 브랜치 이름)` 을 입력한다.
10. `git status` 로 잘 커밋 되었는지 확인하고 github으로 돌아가 결과를 확인 후 pull request 를 클릭한다.
11. 콜라보레이터를 지정하고 코드리뷰 요청을 보낸다 
