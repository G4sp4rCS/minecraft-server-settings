# 🌍 Configuraciones del Servidor Minecraft 🌍

¡Este repositorio te permite levantar servidores de Minecraft de una manera fácil y rápida! 🚀

📚 **Documentación:** [Docker Minecraft Server](https://docker-minecraft-server.readthedocs.io/en/latest/)

## 🛠️ Uso del CLI del Servidor 🛠️

Para usar la interfaz de línea de comandos (CLI) del servidor, ejecuta el siguiente comando:
```sh
docker exec -i 85b8fcb4c1f4 rcon-cli
```

## 📬 Enviando Comandos 📬
RCON está habilitado por defecto, por lo que puedes ejecutar exec en el contenedor para acceder a la consola del servidor Minecraft:

```sh
docker exec -i mc rcon-cli
```

### ⚠️ Nota: El parámetro -i es necesario para el uso interactivo de rcon-cli.

Para ejecutar un comando sencillo, como detener un servidor Minecraft, pasa el comando como argumentos a rcon-cli, así:

```sh
docker exec mc rcon-cli stop
```

En este caso, no se necesita el -i.

Si RCON está deshabilitado, puedes enviar comandos pasándolos como argumentos al script empaquetado mc-send-to-console. Por ejemplo, puedes dar permisos de operador a un jugador en el contenedor mc con:

```sh
docker exec mc mc-send-to-console op player
```

Donde:

mc es el nombre del contenedor.
op player son los comandos de Minecraft.
Puedes copiar y pegar el contenido anterior en el archivo README de tu repositorio o en cualquier otro lugar donde desees presentar esta información. ¡Espero que sea lo que estabas buscando!




