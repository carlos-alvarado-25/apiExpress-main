# Pasos para iniciar el proyecto

#### Clonar el repositorio

```
https://github.com/carlos-alvarado-25/apiExpress-main.git
```

En la carpeta del proyecto iniciar los submódulos con los comandos:
```
git submodule init
```
```
git submodule update
```

Cambiar cada submódulo a una rama funcional (main o develop)

En la raíz del proyecto ejecutar:
```
docker compose up -d --build
```

Ejecutar el contenedor de la base de datos con:
```
docker exec -it mongodb bash
```

Dentro del contenedor ejecutar el comando:
```
mongorestore --db ApiExpress backup
```

Disfrutar del proyecto!!!