## Youtube 소개 영상
https://www.youtube.com/watch?v=mYDVNNUPe6I

## 소개 자료 [pdf]
https://drive.google.com/file/d/1e261cdIq3NJveBo9ooKga28qG2D1P-lk/view?usp=sharing


# project5
### 프로젝트 기술 안내
* Spring MVC
* AJAX(Gantt Chart,Full-Calendar,칸반보드, Google Charts)
* 다국어처리
* SMTP 메일 전송
* 채팅
* JSTL

### 프로젝트 소개
프로젝트 관리 시스템(PMS System)
계획, 조직, 관리하는 것을 도와주고 , 리소스 추산치를 만드는 시스템

### 구현 범위
![image](https://user-images.githubusercontent.com/59445197/160097556-e36235b6-8591-42db-82c9-82feb05a13ad.png)

### 프로젝트 기능
#### 주요 기능
![image](https://user-images.githubusercontent.com/59445197/160097369-3601e890-180d-43ef-88f5-49abe75f7a8c.png)




#### 회원
1. 로그인
* 세션 처리
2. 회원가입
* 가입 신청시 관리자 승인 후 입력 이메일로 임시 아이디/비밀번호 발급
3. 아이디/비밀번호 찾기
* 아이디는 화면에 출력해주시만, 비밀번호는 새로운 비밀번호를 발급하여 이메일로 전송
4. 회원정보 수정
* 이미지 변경
* 아이디 중복검사
* 비밀번호 일치 여부 검사


### PM 페이지
1. 프로젝트
*프로젝트 시작 종료
2. 크롤링 서비스
* 크롤링


## ADMIN 페이지
1. 회원 리스트
* 회원 리스트
* 체크박스 메일 전송

## 프로젝트 대시보드
* 구글 차트


## 칸반/간트/캘린더
* 칸반 CRUD, 드래그 이동
* 간트 CRUD, 드래그 이동
* 캘린더 CRUD, 드래그 이동


#### 리스크
1. 게시글 목록 화면
* 페이징 처리 - 상단의 게시글 수 Select Box의 값과 일치하게 페이징 처리
* 검색 처리 - 프로젝트명, 리스크, 작성일, 완료예정일, 중요도, 진행사항, 담당자를 기준으로 검색
* 전체 게시글 개수 - 검색 시에도 검색된 게시물 만큼 출력
* JSTL을 이용하여 분기 처리한 중요도 및 진행사항 출력
2. 등록
* 등록 버튼 클릭 시 출력되는 모달을 활용한 등록화면
* Select 쿼리를 통한 프로젝트 리스트를 SelectBox에 출력
* Session을 이용한 담당자 Insert 처리
3. 상세화면
* 작성자가 아닐 시 수정, 삭제 버튼 hide
* JSTL을 이용하여 분기 처리한 중요도와 진행도
* 답글 버튼 클릭 시 댓글 작성 form hide, 답글 작성 form show
* 댓글 기능 - 작성자가 아닐 시 댓글 삭제 버튼 hide
* 답글 기능 - 작성자가 아닐 시 댓글 답글 버튼 hide
4. 수정
* input value에 리스크 게시물에 해당되는 키 값을 조건으로 데이터를 가져와 할당
5. 삭제

#### 예산
1. 게시글 목록 화면
* 페이징 처리 - 상단의 게시글 수 Select Box의 값과 일치하게 페이징 처리
* 검색 처리 - 프로젝트명을 기준으로 검색
* 전체 게시글 개수 - 검색 시에도 검색된 게시물 만큼 출력
* JSTL을 이용하여 분기 처리한 예산배정 출력
2. 등록
* 동적 테이블 추가 및 삭제
* 계산 기능
* 프로젝트 선택 시 해당 프로젝트의 예산 출력
* Not in 쿼리를 이용하여 예산 게시판에 작성된 프로젝트는 제외하고 Select
* 리스트에 데이터를 담아 mapper에서 foreach를 통한 동적 테이블의 데이터 insert
3. 상세화면
* 승인 버튼 클릭시 승인 상태로 update
* 프로젝트의 예산 금액과 작성한 예산 데이터의 계산 기능
* JSTL을 활용하여 승인,미승인 출력
4. 수정
* input value에 리스크 게시물에 해당되는 키 값을 조건으로 데이터를 가져와 할당
* 동적 테이블 추가 및 삭제
* merge 쿼리를 이용하여 행 추가 시 insert 기존 행 수정 시 update 처리
* 계산 기능
* 행 데이터 삭제 기능
5. 삭제
* 예산 게시글 테이블의 데이터와 예산 상세정보 테이블의 데이터를 동시 삭제


## 채팅
* 채팅 메시지 삽입
* 채팅 방 불러오기
* 채팅 목록 불러오기
* 소켓 연결
* 1:1 대화 만들기
* 단체 대화 만들기

## 팀관리
1. 프로젝트 배정
* 회원 프로젝트 배정

2. 근태 관리
* 근태 평가
* 경고장 발송

4. 휴가 관리
*휴가 CRUD


## 고객센터/챗봇
1. 고객센터
* 채팅 메시지 삽입
* 채팅 방 불러오기
* 채팅 목록 불러오기
* 소켓 연결
* 1:1 대화 만들기
* 단체 대화 만들기

2. 챗봇
* 정해진 데이터 전송시 일괄적 대답 전송
* 소켓 연결


##
## 프로젝트 역할
* 최윤진 - 회원/관리자/차트/칸반/간트/채팅
* 마혜민 - 인력관리
* 문재영 - 조달관리
* 신지호 - 품질관리
* 윤혜정 - 회의록
* 장훈주 - 예산-ALL, 리스크-ALL, 품질-품질평가, 인증서 발급


### 버전
* 1.0
* 1.1 (22.04.06)