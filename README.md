# Crea tu propio asistente virtual con RASA

## Instalación

Para instalar localmente, ver los [RASA Docs](https://rasa.com/docs/rasa/user-guide/installation/)

Si no quieres instalar RASA en tu computadora y prefieres correrlo en docker, estos son los comandos 

### Entrenar con docker
```docker run -v $(PWD):/app rasa/rasa:1.9.6-full train  ```

Entrenamos usando la versión 1.9.6 con todos los paquetes. 

El modelo quedará guardado en la carpeta ```./models```





### Correr con docker
```docker run -v $(PWD):/app -p 5005:5005 rasa/rasa:1.9.6-full run --enable-api -vv```

Recuerda correr este comando dentro del mismo directorio o el contenedor no podra encontrar el modelo que entrenaste en el paso anterior. 

Con ```--enable-api``` podemos hablar con el bot desde un servicio externo.

Con ```-p 5005:5005``` abrimos el puerto 5005 a la máquina host, lo que nos permite acceder al servidor de RASA.

```-vv``` corre en modo debug completo, de esta manera podemos ver en detalle lo que pasa.


