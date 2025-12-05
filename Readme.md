## Instrucciones para levantar el proyecto

Sigue estos pasos para clonar el proyecto, inicializar los submódulos y levantar los servicios con Docker Compose:

---

### 1️⃣ Clonar el proyecto

```
git clone https://github.com/sistemasfactosys/ProyectoNova.git
cd ProyectoNova
```

---

### 2️⃣ Inicializar los submódulos

```
git submodule update --init --recursive
```

> Esto descargará todos los submódulos usados por el proyecto.

---

### 3️⃣ Levantar los servicios con Docker Compose

```
docker-compose up --build
```

* Para levantar en **segundo plano**:

```
docker-compose up --build -d
```

* Verifica que los contenedores estén corriendo:

```
docker ps
```

* Accede a la app en tu navegador usando el puerto definido en tu `.env` (por ejemplo: `http://localhost:3000`).
