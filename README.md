# p2-t1-vscode-sytws_practica_2_elena

1. Install SNAP

```
sudo apt install snapd
```
```
$ snap --version
snap    2.42.1+18.04
snapd   2.42.1+18.04
series  16
ubuntu  18.04
kernel  4.15.0-108-generic
```

Test

```
$ sudo snap install hello-world
2020-06-28T13:19:01+01:00 INFO Waiting for restart...
hello-world 6.4 from Canonical✓ installed
```

Problem
```
La orden no se pudo encontrar porque «/snap/bin» no está incluida en la variable de entorno PATH.
```

Solution
```
sudo vi /etc/environment
```
add ``` :/snap/bin```

Result
```
# hello-world
Hello World!
```

2. Install Visual Studio Code

**Ubuntu 1804**

```
sudo snap install --classic code
```

Ubuntu 1804 --> Ejecutar --> code
![VSCode](/images/code.png)

```
$ code --version
1.46.1
cd9ea6488829f560dc949a8b2fb789f3cdc05f5d
x64
```

**Mac**

https://code.visualstudio.com/docs/setup/mac
+ Install Extentions from recommended list 

```
$ code --list-extensions
eamodio.gitlens
```

+ Use command line for creating a new file

```
code newfile.js -n
```

![VSCode :IntelliSense](/images/IntelliSense.png)


Working with Github

+ Install *GitHub Pull Requests and Issues* extention
+ Log in 

![VSCode :GitHub](/images/github.png)

+ Git Clone 

![VSCode :GitClone](/images/gitclone.png)

+ Use Integrated Terminal

3. Join Life Share 

+ Install *Live Share Extension Pack*

![VSCode :LifeShare](/images/lifeshare.png)

+ start Session 

Invite Link:
https://prod.liveshare.vsengsaas.visualstudio.com/join?5BFB0575E0B01BF2D592FCA36A3C86E3D96B

4. SSH FS: File system provider using SSH

+ Install *SSH FS* extention
+ Configure remote server --> *Create a SSH FS configuration*
![VSCode :SSH FS](/images/ssh.png)

+ Add remote server data
![VSCode :SSH FS](/images/conf.png)

+ Launch connection  --> *Connect as Workspace folder*
![VSCode :Remote Server](/images/remote_server.png)

