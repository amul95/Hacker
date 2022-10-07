# 1. How many TCP ports are open?
> Nmap se scan krenge machine IP ko aur check krenge ki kitne ports open hai 
    
    ┌─[amul@Hacker]─[~]
    └──╼ $sudo nmap -Pn 10.129.114.197
    Starting Nmap 7.80 ( https://nmap.org ) at 2022-10-07 16:54 IST
    Nmap scan report for 10.129.114.197
    Host is up (0.31s latency).
    Not shown: 998 closed ports
    PORT   STATE SERVICE
    22/tcp open  ssh
    80/tcp open  http

    Ans is : 2 

# 2. What is the domain of the email address provided in the "Contact" section of the website?
> Question me hi website ka zikr hua hai mtlb jo bhi humara machine_ip hai usse hum ek baar URL pr type kre dekhna chahiye koi website hai yaa nhi 
![image](https://user-images.githubusercontent.com/38901699/194543205-8010bdab-2b83-4971-8a70-7656e5186f3c.png)
> app upr image me dekh skte ho ki webiste open hua aur usme "Contacts" ka tab tha uspr mene click kiaa toh ans mil gya ki kya domain name hai email me 
          
    Ans is : thetoppers.htb
    
# 3. In the absence of a DNS server, which Linux file can we use to resolve hostnames to IP addresses in order to be able to access the websites that point to those hostnames?
> Ye hume pata hi hai bhot easy hai hum koi IP address ko kisi name search krna chahte hai toh hum kya krte hai DNS aur locally use krna hot toh apne hisab se toh hum krte hai hosts file config
      
        Ans is : /etc/hosts
        # me 0.0.0.0 ip ke samne amul.com likh dunga toh me fir ping kru amul.com tohwoh 0.0.0.0 ko find krega ab smjhe 
        
# 4. Which sub-domain is discovered during further enumeration?
      Ans is : s3.thetoppers.htb
      
# 5. Which service is running on the discovered sub-domain?
      Ans is : aws s3 ls
# 6.       

