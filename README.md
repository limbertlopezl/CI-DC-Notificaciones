![Ansible Docker](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)
# Integracion Continua Notificacion a Telegram
Despliegue continuo notificacion Telegram (gitlab + ansible+ CI+DC+Docker)
## configuraciones de los parametros de telegram
```
telegram:
          token: 'token_telegram'
          chat_id: idchat del grupo donde enviara los mensajes.
          msg: tu mensaje        
```

## configuraciones gitlab CI/DC
debes ir a esta direccion:https://gitlab.com/CI-DC/Notificaciones-Bots-ci-di/settings/ci_cd de tu proyecto.
y crear la variable SSH_PRIVATE_KEY con tu llave privada de tu servidor.
```
 - ssh-add <(echo "$SSH_PRIVATE_KEY")
```


## Captura de las notificaciones en telegram
<img src="https://github.com/limbertlopezl/CI-DC-Notificaciones/blob/master/img1.jpg" width="400" height="600"/>
