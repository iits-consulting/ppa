 # <img src='https://iits-consulting.de/wp-content/uploads/2021/08/iits-logo-2021-red-square-xl.png' width=150/> otc-auth PPA 
 This repo (based on the one [here](https://github.com/assafmo/ppa)) contains .deb files built from the [latest version of otc-auth](https://github.com/iits-consulting/otc-auth/releases).

 ## Usage 
 ```bash 
 sudo curl -SsL -o /etc/apt/trusted.gpg.d/otc-auth_ppa.gpg https://iits-consulting.github.io/ppa/debian/KEY.gpg 
 sudo curl -SsL -o /etc/apt/sources.list.d/otc-auth.list https://iits-consulting.github.io/ppa/debian/otc-auth.list 
 cat /etc/apt/trusted.gpg.d/otc-auth_ppa.gpg | gpg --dearmor | tee /etc/apt/trusted.gpg.d/otc-auth_ppa.gpg >/dev/null 
 sudo apt update 
 sudo apt install otc-auth 
 ```
