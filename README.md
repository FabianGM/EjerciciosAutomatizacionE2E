# Proyecto de Automatización QA

Este repositorio contiene dos ejercicios de automatización:

1. **Ejercicio UI (SauceDemo con Serenity BDD, Gradle y Cucumber)**
2. **Ejercicio API (PetStore con Karate y Maven)**

Cada carpeta tiene su propio `README.md` explicando su estructura y propósito.

---

## 📂 Estructura del repositorio
ProyectoQA/ ├─ saucedemo-serenity/ │   ├─ README.md │   └─ src/... ├─ petstore-karate/ │   ├─ README.md │   └─ src/... └─ README.md (este archivo)


---

## 🚀 Cómo ejecutar cada ejercicio

- **SauceDemo (UI):**
  - Requiere JDK 11, Gradle 8.14, ChromeDriver.
  - Ejecutar: `gradlew clean test`
  - Reporte: `target/site/serenity/index.html`

- **PetStore (API):**
  - Requiere JDK 11, Maven 3.9.x, Karate 1.4.0.
  - Ejecutar: `mvn clean test`
  - Reporte: `target/karate-reports/karate-summary.html`

---


# Ejercicio UI - SauceDemo con Serenity BDD

Este proyecto automatiza el flujo de compra en [SauceDemo](https://www.saucedemo.com/) usando **Serenity BDD + Cucumber + Gradle**.

---

## 📂 Estructura
saucedemo-serenity/ ├─ src/test/java/com/nttdataprueba/saucedemo/ │   ├─ stepdefinitions/ │   ├─ tasks/ │   ├─ questions/ │   ├─ runners/ │   └─ features/ └─ build.gradle


---

## 🚀 Ejecución

```bash
gradlew clean test

📌 Casos cubiertos
- Login válido
- Agregar productos al carrito
- Checkout exitoso
- Mensaje de confirmación
- Escenario adicional: login inválido

---

### 📄 petstore-karate/README.md

```markdown
# Ejercicio API - PetStore con Karate

Este proyecto prueba la API de [PetStore](https://petstore.swagger.io/) usando **Karate + Maven**.

---

## 📂 Estructura

petstore-karate/ ├─ pom.xml ├─ karate-config.js ├─ src/test/java/petstore/ │   ├─ PetstoreRunnerTest.java │   └─ petstore.feature


---

## 🚀 Ejecución

```bash
mvn clean test

📌 Casos cubiertos
- Añadir mascota (POST /pet)
- Consultar mascota por ID (GET /pet/{id})
- Actualizar mascota a "sold" (PUT /pet)
- Consultar por estatus (GET /pet/findByStatus





