<a href='https://github.com/Junwu0615/NGROK-Dockerization'><img alt='GitHub Views' src='https://views.whatilearened.today/views/github/Junwu0615/NGROK-Dockerization.svg'> 
<a href='https://github.com/Junwu0615/NGROK-Dockerization'><img alt='GitHub Clones' src='https://img.shields.io/badge/dynamic/json?color=success&label=Clone&query=count_total&url=https://gist.githubusercontent.com/Junwu0615/2792e35583530c4e1c58662bbb5a49da/raw/NGROK-Dockerization_clone.json&logo=github'> <br>
[![](https://img.shields.io/badge/Project-Ngrok-blue.svg?style=plastic)](https://github.com/Junwu0615/NGROK-Dockerization) 
[![](https://img.shields.io/badge/Project-Docker-blue.svg?style=plastic)](https://github.com/Junwu0615/NGROK-Dockerization)
[![](https://img.shields.io/badge/Operating_System-Windows_10-blue.svg?style=plastic)](https://www.microsoft.com/zh-tw/software-download/windows10) <br>

<br>

## Dockerization

### *Directory Structure Diagram*
```commandline
NGROK-Dockerization/docker
  └── script
      ├── .env
      └── docker-compose.yaml
```

### *STEP.1　進入腳本路徑*
```bash
cd docker
```

### *STEP.2　新增檔案 : `./script/.env`*
```commandline
NGROK_AUTHTOKEN=<Your Auth Token>
```

### *STEP.3　安裝 docker-compose*
```bash
docker stack deploy -c script/docker-compose.yaml ngrok-dockerization
```

### *STEP.4　檢視 docker service 清單*
```bash
docker service ls
```

### *STEP.5　查看專案 log 打印*
```bash
docker service logs -f ngrok-dockerization_task
```

![00.jpg](/sample/00.jpg)
