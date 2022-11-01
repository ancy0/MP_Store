# 20213024 안채영 개인과제 구현 내용
## 첫번째 화면 (로그인 페이지)
-앱 접속 페이지, 회원 ID/비밀번호(EditView), 로그인/회원가입(Button) 모두 구현
-첫번째 화면 초기화시에 기존에 저장된 개인정보를 preference를 이용해서 읽어 옴
- ID, 비밀번호 입력 시 기존에 가입한 회원 ID, 비밀번호 체크 
-입력한 ID, 비밀번호  오류 시 에러 메시지 출력, 입력값 지움
- ID, 비밀번호 입력이 정상이고 로그인 버튼 클릭 시 세번째 페이지 이동
- 회원가입 없이도 Main 버튼을 클릭하면 세번째 화면으로 이동 가능

## 두번째 화면 (회원가입 페이지)
- 첫번째 페이지에서 회원가입 버튼 클릭 시 출력
- ID 중복검사 구현, 중복검사 하지 않으면 회원가입 불가
- 회원가입 버튼 클릭 시 비밀번호 입력 조건 확인, 조건 불충족 시 회원 가입 불가
- ID, 비밀번호, 이름, 전화번호, 주소 입력확인하여 비어있으면 회원가입 불가 
- 개인정보 사용 동의 간략 약관 동의했을 경우만 가입 가능하도록 구현
- 프레퍼런스(Preference), 파일을 활용하여 회원정보를 저장하고 첫번째 페이지로 이동  
- 모든 회원가입 불가의 경우 Toast문 출력하도록 함

## 세번째 화면(- 상품명, 상품이미지 리스트를 보여주는 화면)
- 5개의 상품의 이미지와 상품명을 기본으로 출력
- 하단의 회원정보 버튼 클릭 시 회원인 경우는 가입한 회원 정보를 보여줌
- 회원이 아닌 경우는 회원정보 버튼을 클릭하면 회원가입 희망 여부에 따라  회원가입 버튼 클릭 시 회원가입 페이지인 두번째 화면으로 이동
- GridView, Text View, ImageView 활용하여 화면 구성
