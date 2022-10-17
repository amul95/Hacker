Hum dekhenge gubuster jo command hai woh use krte hai kali-linux me use krte hai toh koi error nhi aata par jese hum ubuntu me use krte hai toh woh nhi hota hai sahi 
se work toh uska solution bas itna hai ki jo hum "sudo apt install gobuster" install krte hai toh woh latest version nhi aata hai isliye hume personally lateset version 
download krna padega toh uski link niche di hai 
  
  
      https://github.com/OJ/gobuster/releases/tag/v3.2.0
      # Fir scroll krna hai usme aapko ye wali file dikhegi gobuster_3.2.0_Linux_x86_64.tar.gz jo ubuntu pr work kregi usse download kr lo 
      
      tar -xvf gobuster_3.2.0_Linux_x86_64.tar.gz
      # aese krke us file  ko unzip kr do 
      
      > Unzip ke baad total 3 jise extract hogi 
        gobuster
        Readme.md
        Licence
      > bas ab jis folder me extract kie ho aap wnha jaakr janha ye 3 file dikhe usmme simple sa command do 
      
        /gobuster dir -w /usr/share/payloads/SecLists/Discovery/Web-Content/directory-list-2.3-medium.txt -u http://photobomb.htb/
        
        #ab dekhoge ki koi error nhi aayega aur work  bhi krega ubuntu me gobuster tool pr haan /gobuster aese hi likhna 
