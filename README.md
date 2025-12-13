# MC-SERVER-GLOBAL

El fin de repositorio es mantener centralizado las configuraciones para un server de minecraft utilizando docker y playit-gg, utilizando un archivo de docker-compose.

**Enlaces útiles**
- [Imagen de docker a utilizar + Documentación oficial](https://github.com/itzg/docker-minecraft-server) 
- [playit-gg](https://playit.gg/) 


## Configuración

_Las customizaciones principales se encuentran en el archivo `.env` y tratar de no tocar el `docker compose`._

1. **Clonar el repositorio**

```
git clone https://github.com/ianchu0317/mc-server-global.git
```

2. **Configurar agente Docker de Playit-GG**

Ir a [playit-gg](https://playit.gg/) y crear un agente docker. Copiar SECRET TOKEN y poner en `.env`.


3. **Configurar Túneles**

Al agente docker crear dos túneles distintos. 
El primer túnel utilizando modo de juego JAVA apuntando a puerto `25565` y el segundo con modo de juego BEDROCK apuntando `19132`.

4. **Iniciar servidor**

```
docker compose up -d
```


## Conexión

Para conexión global utilizar los enlaces que muestra en plataforma.

Para conexión local se puede acceder en:

```
- <ip>:25565 (JAVA)
- <ip>:19132 (BEDROCK)
```