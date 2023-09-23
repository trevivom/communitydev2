# 게시판 만들기
간단히 사용자들과 소통할 수 있는 게시판 서비스를 만드는 개인프로젝트
# 프로젝트 기능 및 설계


- 회원가입 기능
	- 사용자는 회원가입을 할 수 있다. user권한을 가진다.
	- 회원가입시 아이디와 패스워드를 입력받고, 아이디는 중복되선 안된다.

- 로그인 기능
	- 사용자는 로그인을 할 수 있다.로그인시 회원가입때 사용한 아이디와 패스워드가 일치해야한다.
	
- 게시글 작성 기능
	- 로그인한 사용자는 글을 작성할 수 있다.
	- 사용자는 제목(텍스트), 내용(텍스트)을 작성할 수 있다.

- 특정 게시글 조회 기능
	- 로그인하지 않은 사용자를 포함한 모든 사용자는 게시글을 	조회할 수 있다.
	- 게시글 제목, 내용, 작성자, 작성일, 댓글 목록이 조회된다.

- 게시글 목록 조회 기능
	- 모든 사용자는 게시글을 조회할 수 있다.
	- 게시글은 최신순으로 기본 정렬되며, 댓글수순, 조회수순	으로도 정렬이 가능하다.
	- 게시글 목록 조회시 응답에는 게시글 제목과 작성일, 댓글 	수의 정보가 필요하다
	- paging 처리.
   
- 게시글 수정 기능
	- 로그인하여 글을 작성한 사용자는 작성한 글을 수정할 수 있	다.
	- 제목(텍스트), 내용(텍스트)을 수정할 수 있다.

- 게시글 삭제 기능
	- 로그인하여 글을 작성한 사용자는 작성한 글을 삭제할 수 있	다.

- 댓글 목록 조회 기능
	- 특정 게시글 조회시 댓글목록도 함께 조회가 된다. 댓글은	별도의 API로 구성한다. 모든 사용자가 댓글을 조회할 수 있	다.
	- 댓글은 최신순으로 정렬되며, paging처리를 한다.
	- 댓글 목록 조회시 댓글 작성자와 댓글 내용, 댓글 작성일의 	정보가 필요하다.

- 댓글 작성 기능
	- 로그인한 사용자는 권한에 관계 없이 댓글을 작성할 수 있다.
	- 댓글은 내용(텍스트)을 작성할 수 있다.
	
- 댓글 수정 기능
	- 댓글을 작성한 사용자는 댓글을 수정할 수 있다.
	- 내용(텍스트)을 수정할 수 있다.

- 댓글 삭제 기능
	- 댓글을 작성한 사용자는 댓글을 삭제할 수 있다.

# ERD
![erd_dev1](https://github.com/trevivom/communitydev2/assets/107251548/9880879c-f6d7-44e4-87d5-956b3a845144)


## Trouble Shooting
[go to the trouble shooting section](trouble_shooting.md)

# Tech Stack
JAVA, SPRING, JPA, MYSQL, GIT
