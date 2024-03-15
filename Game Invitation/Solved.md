![image](https://github.com/anhshidou/HTB2024/assets/120787381/07bf5492-8fc0-422c-b1d8-004072d0a14f)At this question, it kinda hard but I still can solve it hehe

![image](https://github.com/anhshidou/HTB2024/assets/120787381/ae1c28bb-f3f3-4d4a-9b6d-eacd22fd8f2a)

To do it, you must know about macro, however, for starting it, first thing will be turn off the window defender and using the docm file

First start, you must unblock the macro and set permissions to full use

![image](https://github.com/anhshidou/HTB2024/assets/120787381/099133cd-afc1-4639-b26a-c87c779f005e)

Now we will step to part 2

![image](https://github.com/anhshidou/HTB2024/assets/120787381/99e1fd06-bfae-4638-b252-687ef498e39c)

As we can see, we get the VBA script that are usually used for writing macro

![image](https://github.com/anhshidou/HTB2024/assets/120787381/9e700647-bc1b-4f0c-b8f6-22f01a09db34)

Now, we must fix the script

First thing go to my eyes is the sub AutoClose() it sounds like its function is going to delete the file so that I will remove it

After that, we can see the condition, if chkDomain != strUserDomain then it doesn't run anything so that we will fix it by remove the Else part in order to make the run go through

![image](https://github.com/anhshidou/HTB2024/assets/120787381/8d7c8350-c836-4049-a9c0-336914d47a07)

![image](https://github.com/anhshidou/HTB2024/assets/120787381/f1b1c394-a167-47ab-adbc-de209dd9c589)

After that, we set up breakpoint by using F8 at this point

![image](https://github.com/anhshidou/HTB2024/assets/120787381/ab89485a-a85e-41fe-b58d-73c7a4e46136)

It will return the file is mailform.js

![image](https://github.com/anhshidou/HTB2024/assets/120787381/b14e8f98-9b7e-4631-ada6-34f78dc87269)

We will find the flag in base64 

![image](https://github.com/anhshidou/HTB2024/assets/120787381/efbe9145-268e-4df6-bbd2-d98220eb4641)

Flag when we decoded:

![image](https://github.com/anhshidou/HTB2024/assets/120787381/59e9dd30-c31c-4adc-a3b4-01bbb94e7391)

Flag: HTB{m4ld0cs_4r3_g3tt1ng_Tr1cki13r}
