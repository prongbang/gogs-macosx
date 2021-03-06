# gogs-macosx

# Requirement

- https://www.docker.com/products/docker-desktop


## 1. Mac - Clone this repository

```
$ git clone https://github.com/prongbang/gogs-macosx.git
```

## 2. Mac - Run Server

```
$ cd gogs-macosx
$ make run

or

$ docker-compose up -d
```

## 3. Mac - Setup

- เปลี่ยน IP `127.0.0.1` เป็น `gogs-db` 

- http://localhost:3000/install

- User Database
```
user: root
pass: admin
db: gogs
```

![Screenshot png](screenshot/setup.png)

## 4. Mac - Register

## 5. Mac - Sign In

## 6. Mac - Create Repository

## 7. Mac - Git Add Remote Local Repository

```
$ git add remote local http://git-server-ip:3000/username/repository-name.git

or

$ git add remote local http://localhost:3000/username/repository-name.git
```

#### How to get `git-server-ip`

- Open terminal

```
$ ifconfig
```

Output 

```
en0: ...
     inet xxx.xxx.xxx.xxx
```

- Click Wifi -> Open Network Preferences....

```
Wi-Fi is connected to WifiName and has the IP address xxx.xxx.xxx.xxx
```

## 8. Mac - Push to local remote repository

```
$ git push -u local
```

## 9. Windows - (Connect VPN) Git Clone Project from Internal 

```
$ git clone https://git-internal-ip/username/repository-name.git
```

## 10. Windows - Add Remote to git local repository (Mac)

```
$ git add remote local http://git-server-local-ip-mac:3000/username/repository-name.git
```

## 9. Windows - Git pull on Windows

```
$ git pull local
```

## 10. Windows - (Connect VPN) Git push to Internal

```
$ git push
```


## Summary

### Windows 

- Remote

```
origin    -> https://git-internal-ip/team/repository-name.git
m         -> https://git-internal-ip/username/repository-name.git
local     -> https://git-server-local-ip-mac:3000/username/repository-name.git
```

- Pull from Local

```
$ git pull local
```

- Pull from origin

```
$ git pull origin
```

- Push to m

```
$ git push -u m
```

- New Merge Request

```
m/feature/name -to-> origin/develop 
```

- Pull from origin

```
$ git pull origin
```

- Push to local

```
$ git push -u local
```

### Mac 

- Remote

```
origin    -> https://localhost:3000/username/repository-name.git
```

- Pull from local

```
$ git pull
```

- Push to local

```
$ git push
```
