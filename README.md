# Hacker

# Hack The Box
-- mene start kia hai hack the box ka starting point aur jitne bhi usme task hai aur machines hai woh hum sb milkar spawn karenge aur uske bich muje jo personally dikkt hui woh hi me share krunga aur solution dunga kyun ki woh pura aapko Walkthrough mil jayega kahi se bhi but uske baad bhi kuch kuch dikkt hoti hai isliye me ye bana rha hoon....auer uske alwa chote chote topic jo hume pata hone chahiye 

# WinSCP
> muje mere ubuntu ke terminal se kisi aur jagh me rkhe hue ubuntu desktop se file copy krvani hai kese krunga like filezilla yaa WinSCP se me pnetlab me kyaa krta thaa yaad hai ?? drag krke opt wale bin yaa iul me images copy krta tha pr me kahu ki muje winscp ka jo graphical user ke bina sirf terminal se hi krna hai toh kese krenge chlo dekhte hai 
> mene linode pr ek kali-linux ka instance banaya hua hai aur me usse access krunga apne ubuntu local se 
> aur fir hum local ubuntu se usme kuch copy krenge aur wnha linode wale se humare ubuntu local se kuch copy krvayenge 
> Let's go...
![image](https://user-images.githubusercontent.com/38901699/194249306-bb568cf4-0395-480e-9350-0cd997eb2ac8.png)
> aap upar image me dekh skte ho ki left side mera local ubuntu ka terminal hai means woh mera laptop me jo ubuntu dala hai woh uska hai 
> aur right side me hai kali-linux jo diffrenet hai cloud pr jo mene linode se create kia hai ab hum in dono me file/folder copy krenge sirf terminal ke through let's go...
![image](https://user-images.githubusercontent.com/38901699/194260325-ea05bfce-c5e4-46e2-892c-91d698ce9ff1.png)
>> Dekho up image me jo kali OS hai jo linode pr create kia hai mene usme /root/home/ pr ek text file create kia hai ab muje woh file apne ubuntu pr copy krvani hai 
![image](https://user-images.githubusercontent.com/38901699/194261710-98bab305-f7ea-4786-9f08-23c250fccf4d.png)
>> See, dekhiae upr mene apne wale local ubuntu me kese command use kie hai ab hum smjhe ke ye commad ka mtl kya hai in-depth me 

    scp root@192.46.212.240:/home/test_file.txt /home/amul/Desktop/
    
 **scp**                    >>> ye tool jiske zariae hum copy krvayenge remote_location se apne local system par

 **root@192.46.212.240**    >>> ye hum janha file copy krna chahte hai uska remote_username & remote_ip address

 
 
 **:**                      >>> ye bhot zaruri hai jese hi humara  IP address khtm ho uske baad turnt ye ":" ye 
                                daal do aur uske bad turant path
 
 **/home/test_file.txt**    >>> ye remote_location ka path hai jnha pr file ye actual me hai kali_OS me muje wnha 
                                se apne local ubuntu pr copy krvana hai
 
 
 **/home/amul/Desktop/**    >>> aur end mera wala path hai janha me copy krvana chahta hoon like local path aur aap 
                                upr dekh skte ho ki copy ho chuki hai
    
    "home/test_file.txt"    >>> ye without space likha hua hai toh ye correct hai

    ": /home/test_file.txt" >>> ye space dia hua hai toh ye error show krega 
# Conclution
> aapko smj aya ki kese remote_location se file humre local system par copy krvani hai yaad rhe ki scp commad ke baad turnt  jhna se file copy krni hai uska username fir uska ip address fir fir us system jo file copy krni hai woh wnha kaha pr stored hai woh path aur end me hume humare local pr kaha copy krna hai woh path aayega 

aur agar file ki jgh folder hua toh apko simple -r use krna hai scp command ke baad turnt toh folder bhi copy ho jayega ok woh bhi dekh lete hai humlog practical karke 

![image](https://user-images.githubusercontent.com/38901699/194267135-6432be3b-c059-4b2e-90d6-1440d1fff154.png)
Ab image dekhkr kuch kuch smj aaya hoga sbse pehle mene kali_OS pr ek new_folder banaya aur uske ader woh test file move kr di ab humara task hai ki hum pura ka pura folder copy kre woh kese krenge dekhte hai command sb same hai mene bas -r use kiaa scp ke aage toh dekho older bhi copy ho gya 

aur ek baad pehle wale me mene remote_username root use kia tha pr hum as a username bhi use kr skte hai jese mafia mene use kia woh kali_OS pr mene new user create kia tha toh hm aese bhi likh skte hai root@remote_ip & usename@remote_ip like this bas toh bhot hai itna
    
