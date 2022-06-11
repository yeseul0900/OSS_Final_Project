<h1>What does this project do? </h1>

This project is a resume tool for developers, and you can easily create a sophisticated resume. It is easy to print out what my ability and career are, in what ways they are good, and what development skills they have.

<h1> Why is this project useful? </h1>

Resume is important because it is my first impression of the company. Traditional resumes on the Internet are very cliche. It's hard and it's the same image, and there's a lot of stuff you don't need But this resume is different. 
In addition, it is a good resume that can only appeal to the developer's ability because it only has the necessary items. 
In addition, it is easy to modify items, so you can customize them.

<h1>How to get started? </h1>
It can be difficult to create an environment where you can start. But with a little effort, you can do it easily.
<h2>1. Check the Apt Version.</h2>
   – $ sudo apt-get update<br>
   – $ sudo apt-get upgrade<br>
   – $ sudo apt-get auto remove<br>
<h2>2. Install nginx. </h2>
   - $ sudo apt-get install nginx<br>
   - $ sudo service nginx start<br>
  This page should appear when you put your own ip address in your browser.<br><br>

   <img width="891" alt="Welcome to nginx!" src="https://user-images.githubusercontent.com/103619278/173187273-c4cfa32e-bfab-49b8-8146-ccf759a14ad8.png"><br>
   
<h2>3. Make a New user</h2>
1) 라즈베리 파이에 로그인 한 상태에서 다음 명령어를 입력해 루트로 전환합니다.<br>
    - $ sudo su -<br>
2) 새로운 유저를 만듭니다. <br>
    - $ useradd -m resume<br>
    - $ passwd resume<br>
    - 패스워드 입력<br>
3) 다음 명령어를 입력하여 새로운 유저로 로그인합니다.<br>
    - $ su - resume<br>
4) 다음 레포지토리를 가져오고 권한을 바꿔줍니다.<br>
    - $ git clone <br>
    - $ chmod -R 755 repository_name<br>
    - $ exit<br>
<h2> 4. Make a virtual host</h2>
 1) 루트서버인 것을 확인하고 다음과 같이 실행합니다. <br>
 - $ cd /etc/nginx/sites-available<br>
 - $ cp default resume.com<br>
 - $ vi resume.com<br>
 2) 다음 항목들을 변경합니다. <br>
- Remove default<br>
<img width="242" alt="server {" src="https://user-images.githubusercontent.com/103619278/173187681-b35ab2c3-a564-41e6-8b20-b8b8055217d1.png"><br>
- Change the default root<br>
<img width="176" alt="#root varwwwhtml;" src="https://user-images.githubusercontent.com/103619278/173187687-e2002f76-7c8f-41e2-9b52-e9c5020ac761.png"><br>
- Setting server_name<br>
<img width="385" alt="# Add index php to the list if you are using PHP" src="https://user-images.githubusercontent.com/103619278/173187704-d8411732-21e2-4e58-894c-ce2679679f69.png"><br>
  3) 잘 변경 되었는지 확인하는 방법은 다음과 같습니다.  <br>
<img width="475" alt="nginx the configuration file etcnginxnginx conf syntax is ok" src="https://user-images.githubusercontent.com/103619278/173187757-b6ace9b1-e8db-498b-9ad2-9233046fcc26.png"><br>
  4) Restart The nginx!<br>
<img width="417" alt="(root@ysetcnginxsites-available# service nginx restart" src="https://user-images.githubusercontent.com/103619278/173188218-5339b0fb-da37-4fdd-a388-45f47ac9fbca.png"><br>

  5) 내 터미널에서 다음과 같이 입력합니다. <br>
  - $ sudo vi /etc/hosts<br>
  6) ::1 localhost밑에 다음과 같이 입력합니다. <br>
  - $ yourip resume.com<br>
이렇게 하면 세팅이 완료입니다. <br>

<h2>Vs코드를 이용한 수정</h2>
1) SFTP를 다음과 같이 세팅하고, 비밀번호를 입력합니다. <br>
<img width="307" alt="name My Server," src="https://user-images.githubusercontent.com/103619278/173187893-ffc885e8-8f45-4e06-a08b-ee9a8f28a9e4.png"><br>
2) index.html 파일을 우클릭하여 edit in local을 선택합니다. <br>
3) 컨트롤 f로 edit: 을 검색하면 주석으로 달아둔 수정 가능한 부분들이 나타납니다. 자신의 이력에 맞게 수정하세요.<br>
4) 수정한 파일을 업로드 한 뒤 크롬이나 사파리에 resume.com을 입력하면 내가 현재 작성하는 페이지가 나타납니다.<br>
5) 작성을 완료했다면 페이지에서 우클릭 후 인쇄하면 됩니다.<br>
 
Tip) 프로필 사진을 위한 이미지 파일을 올릴때는 FileZilla를 사용하면 편합니다. <br>
  사이트 관리자 클릭<br>
<img width="293" alt="스크린샷 2022-06-11 오후 9 29 15" src="https://user-images.githubusercontent.com/103619278/173187977-9e6e5b27-1219-4e36-b518-b6ad83c62a52.png"><br>
  new site를 클릭하고 다음과 같이 세팅해주면 됩니다. <br>
<img width="836" alt="스크린샷 2022-06-11 오후 9 29 57" src="https://user-images.githubusercontent.com/103619278/173188249-546f2351-f19e-42d8-911f-58e73155980e.png">


Where can people get more help, if needed?

Presentation Video (YouTube) Link
