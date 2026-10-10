# 🚀 RESTful API & Microservicio PHP (Dockerizado)

[![PHP](https://img.shields.io/badge/PHP-8.2+-777BB4?style=for-the-badge&logo=php&logoColor=white)](https://www.php.net/)
[![Docker](https://img.shields.io/badge/Docker-Enabled-2496ED?style=for-the-badge&logo=docker&logoColor=white)](https://www.docker.com/)
[![REST API](https://img.shields.io/badge/API-RESTful-green?style=for-the-badge)]()
[![CORS](https://img.shields.io/badge/CORS-Configured-blue?style=for-the-badge)]()

Microservicio API REST ligero, autocontenido y dockerizado desarrollado en **PHP**, diseñado para servir datos estructurados a clientes web modernos (React, Vue, SPA) y aplicaciones móviles con soporte completo para CORS y manejo de preflight requests.

---

## ✨ Características

* ⚡ **Cero Dependencias Externas:** PHP puro optimizado para máxima velocidad de respuesta y bajo consumo de memoria.
* 🌐 **Soporte CORS Integral:** Encabezados configurados para `OPTIONS`, `GET` y `POST` con preflight cacheable (`Access-Control-Max-Age`).
* 📦 **Entorno Dockerizado:** Despliegue en un solo comando mediante el `Dockerfile` oficial incluido.
* 🔍 **Estructura de Datos Enriquecida:** Catálogo estructurado con IDs únicos, metadatos, calificaciones, clasificaciones y enlaces a recursos multimedia.

---

## 🛠️ Endpoints Disponibles

| Método | Endpoint | Descripción | Respuesta |
| :--- | :--- | :--- | :--- |
| `GET` | `/` | Retorna el listado completo de registros en formato JSON | `200 OK` (Array JSON) |
| `OPTIONS` | `/` | Manejo de solicitudes preflight de navegadores | `200 OK` (Headers CORS) |

---

## 🐳 Despliegue con Docker

```bash
# 1. Clonar el repositorio
git clone https://github.com/gavafue/API.git
cd API

# 2. Construir la imagen Docker
docker build -t php-api .

# 3. Levantar el contenedor en el puerto 8080
docker run -d -p 8080:80 --name mi-api php-api

# 4. Probar el endpoint
curl http://localhost:8080/
```

---

## 👨‍💻 Autor

* **Gabriel Vázquez** — *Profesor de Informática (INET) & Full Stack Developer*
* [LinkedIn](https://www.linkedin.com/in/gavafue) · [CVUy](https://export.cvuy.uy/cv/?1ef08a58a0c81bcd4d399b62513ffa9a)
