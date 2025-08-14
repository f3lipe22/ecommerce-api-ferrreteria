# 🛒 E-commerce API - Spring Boot

API backend para un sistema de e-commerce desarrollada con **Spring Boot**, **PostgreSQL** y **Docker**.

## 📋 Requisitos previos

- **Java 17+**
- **Maven** (opcional si usas el wrapper `mvnw`)
- **Docker** y **Docker Compose**
- **Git**

---

## 🚀 Configuración de entornos

Este proyecto usa **perfiles de Spring Boot** para separar configuración:

- **`local`** → Desarrollo con Docker (base de datos local).
- **`prod`** → Producción en Render (base de datos externa).

---

## 🛠️ Variables de entorno

Crea un archivo `.env` en la raíz del proyecto para el entorno local:

```env
POSTGRES_DB=ecommerce
POSTGRES_USER=ecommerce_user
POSTGRES_PASSWORD=ecommerce_pass

```

---

## 💻 Despliegue local

- Crear el `.env`
- Levantar base de datos con docker (` docker compose up -d `)
- Ejecutar la aplicación en modo local (` ./mvnw spring-boot:run -Dspring-boot.run.profiles=local
 `)
