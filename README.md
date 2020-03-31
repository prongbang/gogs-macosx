# gogs-macosx

# Requirement

- https://www.docker.com/products/docker-desktop


## 1. Clone this repository

```
https://github.com/prongbang/gogs-macosx.git
```

## 2. Run Server

```
$ cd gogs-macosx
$ make run

or

$ docker-compose up -d
```

## 3. Setup

- ให้เลือกเป็น `PostgreSQL` แทน 
- เปลี่ยน IP `127.0.0.1` เป็น `gogs-db` 

- http://localhost:3000/install

- User Database
```
user: root
pass: admin
db: gogs
```

![Screenshot png](screenshot/setup.png)

## 4. Register

## 5. Sign In

## 6. Create Repository

## 7. Add Remote Repository

```
$ git add remote local http://git-server-ip:3000/username/repository-name.git
```

## 8. Push local repository to remote repository

```
$ git push -u local
```

## 9. Git pull on Windows

```
$ git pull local
```

## 10. Git push to Internal

```
$ git push
```
