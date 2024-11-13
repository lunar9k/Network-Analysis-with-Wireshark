# Network-Analysis-And-Investigation-with-Wireshark

## First we have to gain details of traffic

we have to open the file in wireshark and analyze the traffic 
If any unknown `POST` or `GET` request is send or recive and we also have to check `HTTP` protocall  

![Screenshot (49)](https://github.com/user-attachments/assets/330b7e27-d0fb-46bf-883f-5014d70fcc16)
### I see a `GET` request and `.exe` in fraffic and we have to investigate this 





## Now we can invesigate this in detail 

for this we can filtter `HTTP` request and then open this
![Screenshot (50)](https://github.com/user-attachments/assets/a05b56c7-5639-49ea-989a-0c7bebf56baf)
we can see the malecious link / URI in rhis pictuse of `.exe` file




## we right click and open HTTP stream for view in detail 
we can see the `MZ` and the message called `This programm cannot be run in DOS mode ` this is sign for us it means the file is made for WINDOWS and can run in only windows
and `MZ`  is the first couple bytes of the file, also known as the file signature 
![Screenshot (51)](https://github.com/user-attachments/assets/ad3f1620-a6c5-411c-880a-f519f56ca66e)

## We have search the link in virustotal
we search the link we found in this request and the result is given 
this means the link is malecious and the IP is also malecious , the score is low but that dosent mean the link is little safe it is harmful
![Screenshot (52)](https://github.com/user-attachments/assets/51c2bcba-ad40-4bd3-ac02-8e7704f8e993)


## Conclusion 

Final URL
http://192.227.196.211/FRESH/fresh.exe 

Serving IP Address 192.227.196.211

Body SHA-256
27a210e1d8192d8455595ac2cb4b674f524ac9d329332eb3b36e9277c5185a7d

server
Apache/2.4.52 (Win64) OpenSSL/1.1.1m PHP/8.1.2
  
date Tue, 29 Mar 2022 07:20:17 GMT




