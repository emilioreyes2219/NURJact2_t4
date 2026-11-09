# Aplicación Spring Boot 
Nunez Reyes Jorge Emilio

## 🛠️ Endpoints y Vistas del Proyecto

### 1. Vistas Thymeleaf (MVC)
* **Lista de Empleados (`th:each`):** `http://localhost:8080/detalles_info`
* **Formulario de Registro (`@ModelAttribute`):** `http://localhost:8080/form` *(Envía datos por POST a `/guardar`)*

### 2. Endpoints REST (JSON)
* **DTO:** `http://localhost:8080/api/detalles_info2`
* **Query Parameters (`@RequestParam`):**
  * Detalle: `http://localhost:8080/api/parametros/detalle?informacion=TextoPrueba`
  * Saludo: `http://localhost:8080/api/parametros/saludo?nombre=Jorge`
* **Path Variables (`@PathVariable`):**
  * Mensaje: `http://localhost:8080/api/variable/pagina1/MiMensaje`
  * ID Empleado: `http://localhost:8080/api/variable/empleado/1`
* **Propiedades personalizadas (`@Value`):** `http://localhost:8080/api/variable/valores`
* **Petición POST (`@RequestBody`):** `http://localhost:8080/api/variable/solicitud` *(Probar en Postman/Bruno enviando un JSON de Empleado)*

### 3. Identificación en el VPS
* **Instancia Activa:** `http://localhost:8080/mi-instancia` *(Ajustar al puerto `8085` en el VPS)*