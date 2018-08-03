# Docker Compose

Name your containers and network. Depending on default names might cause trouble sometimes.

```yml
services:
  redis:
    container_name: entrytask_redis

networks:
  ntw:
    name: entrytask_ntw
```
