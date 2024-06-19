# Blurry-writeup-HTB
Let's perform an nmap scan

```bash
nmap -sCV -A 10.10.11.19
```

![alt text](https://github.com/Milamagof/Blurry-writeup-HTB/blob/635246a4b8ec31bab83424e0ec2dc9a1dbe30462/Screenshot_2024-06-08_15_45_41.png)

We must add the subdomains:

```bash
sudo nano /etc/hosts 
```

![alt text](https://github.com/Milamagof/Blurry-writeup-HTB/blob/52f9e337e18d4ba5b6940ca24728b4df07d5d6a1/Screenshot_2024-06-10_18_45_06_1.png)


Let's visit the web port app.blurry.htb that we discovered with the nmap scan


![alt text](https://github.com/Milamagof/Blurry-writeup-HTB/blob/52f9e337e18d4ba5b6940ca24728b4df07d5d6a1/Screenshot_2024-06-08_15_46_05.png)

Just by entering a username we can enter.

![alt text](https://github.com/Milamagof/Blurry-writeup-HTB/blob/52f9e337e18d4ba5b6940ca24728b4df07d5d6a1/Screenshot_2024-06-08_16_28_06.png)


-

![alt text]()


-

```javascript

```


![alt text]()

-

```bash

```

![alt text]()


```bash
```

![alt text]()

-

![alt text]()


-


-

![alt text]()

-

I find [CVE-2022-25912](https://security.snyk.io/vuln/SNYK-JS-SIMPLEGIT-3112221). Let's use this for our payload.

-
```bash

```

![alt text]()

-

![alt text]()


-
-

```bash

```

![alt text]()


```bash

```

![alt text]()

-

![alt text]()


-
```bash
python3 -c 'import pty; pty.spawn("/bin/bash")'
Ctrl+Z
stty raw -echo;fg
export TERM=xterm
export SHELL=bash
```

![alt text]()

-

![alt text]()



```bash

```

![alt text]()


-


```bash

```


user.txt

![alt text]()

-

![alt text]()



-

```bash

```
-

![alt text]()


I find such an [blog](https://community.librenms.org/t/adding-admin-users-on-librenms/20782) to add `admin` user.

-

![alt text]()


-

![alt text]()


-
```bash

```

![alt text]()

-

![alt text]()




![alt text]()

-

![alt text]()



![alt text]()


I find [exploit](https://www.exploit-db.com/exploits/46544), let's use this.



```bash

```

![alt text]()



```bash

```


```bash

```

My `/tmp/shell.sh` file is executed, that's why I get reverse shell from port `1337`.

root.txt

![alt text](img/image-29.png)
