# Game On! Web Webapp

[![Codacy Badge](https://api.codacy.com/project/badge/grade/97dba9bf5a944578b56831a974f225fa)](https://www.codacy.com/app/gameontext/gameon-webapp)

This project contains just the JavaScript web application (no services).

## Docker

### Building

```
docker build -t gameon-webapp
```

### Interactive Run

```
docker run -it -p 3000:3000 --env-file=./dockerrc --name gameon-webapp gameon-webapp bash
```

### Daemon Run

```
docker run -d -p 3:9443 --env-file=./dockerrc --name gameon-webapp gameon-webapp
```

### Stop

```
docker stop gameon-player ; docker rm gameon-player
```

### Restart Daemon

```
docker stop gameon-player ; docker rm gameon-player; docker run -d -p 9443:9443 --env-file=./dockerrc --name gameon-player gameon-player
```


