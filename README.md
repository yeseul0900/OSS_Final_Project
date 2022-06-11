<h1>What does this project do? </h1>

This project is a resume tool for developers, and you can easily create a sophisticated resume. It is easy to print out what my ability and career are, in what ways they are good, and what development skills they have.

<h1> Why is this project useful? </h1>

Resume is important because it is my first impression of the company. Traditional resumes on the Internet are very cliche. It's Boring and the same image, and there's a lot of subject you don't need you. But this resume is different. In addition, it is a good resume that can only appeal to the developer's ability because it only has the necessary items. In addition, it is easy to modify subject so you can customize them.

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
1) While logged in to Raspberry Pi, enter the following command to switch to root.<br>
    - $ sudo su -<br>
2) Create a new user. <br>
    - $ useradd -m resume<br>
    - $ passwd resume<br>
    - Enter Password<br>
3) Log in as a new user by entering the following command.<br>
    - $ su - resume<br>
4) Gets the following repository and changes permissions.<br>
    - $ git clone <br>
    - $ chmod -R 755 repository_name<br>
    - $ exit<br>
<h2> 4. Make a virtual host</h2>
 1) Verify that it is the root server and run as follows <br>
 - $ cd /etc/nginx/sites-available<br>
 - $ cp default resume.com<br>
 - $ vi resume.com<br>
 2) Make the following changes <br>
- Remove default<br>
<img width="242" alt="server {" src="https://user-images.githubusercontent.com/103619278/173187681-b35ab2c3-a564-41e6-8b20-b8b8055217d1.png"><br>
- Change the default root<br>
<img width="176" alt="#root varwwwhtml;" src="https://user-images.githubusercontent.com/103619278/173187687-e2002f76-7c8f-41e2-9b52-e9c5020ac761.png"><br>
- Setting server_name<br>
<img width="385" alt="# Add index php to the list if you are using PHP" src="https://user-images.githubusercontent.com/103619278/173187704-d8411732-21e2-4e58-894c-ce2679679f69.png"><br>
  3) Here's how to check if it's changed well.  <br>
<img width="475" alt="nginx the configuration file etcnginxnginx conf syntax is ok" src="https://user-images.githubusercontent.com/103619278/173187757-b6ace9b1-e8db-498b-9ad2-9233046fcc26.png"><br>
  4) Restart The nginx!<br>
<img width="417" alt="(root@ysetcnginxsites-available# service nginx restart" src="https://user-images.githubusercontent.com/103619278/173188218-5339b0fb-da37-4fdd-a388-45f47ac9fbca.png"><br>

  5) In My Terminal, typing this. <br>
  - $ sudo vi /etc/hosts<br>
  6) Under ::1 localhost, typing this <br>
  - $ yourip resume.com<br>
This completes the setup. <br>

<h2>Modification using Vs code</h2>
1) Set SFTP as follows, and enter the password.<br>
<img width="307" alt="name My Server," src="https://user-images.githubusercontent.com/103619278/173187893-ffc885e8-8f45-4e06-a08b-ee9a8f28a9e4.png"><br>
2) Right-click the "index.html" file and select "edit in local". <br>
3) Search for "edit:" with CTRL+f. This help you know what you edit of Item. Edit it.<br>
4) After uploading the modified file, type resume.com in Chrome or Safari, and the page you are currently creating will appear.<br>
5) When you're done, right-click on the wep page and print.<br>
 
Tip)  It is convenient to use FileZilla when uploading an image file for a profile picture. <br>
  Click the "사이트 관리자"<br>
<img width="293" alt="스크린샷 2022-06-11 오후 9 29 15" src="https://user-images.githubusercontent.com/103619278/173187977-9e6e5b27-1219-4e36-b518-b6ad83c62a52.png"><br>
  Click on the "new site" and set it up as follows. <br>
<img width="836" alt="스크린샷 2022-06-11 오후 9 29 57" src="https://user-images.githubusercontent.com/103619278/173188249-546f2351-f19e-42d8-911f-58e73155980e.png">


<h2>Where can people get more help, if needed?</h2>
1) If you want to know more about resume, please refer to here. The license of the resume used in my project is also here. : https://github.com/xriley/pillar-theme.git<br>
2) If you have any questions. contact to me. 
   My Email adreess is...: yeseul0900@handong.ac.kr

Presentation Video (YouTube) Link
