# Aplicación Spring Boot 
Nunez Reyes Jorge Emilio

## 🛠️ Endpoints y Vistas del Proyecto (VPS)

### 1. Vistas Thymeleaf (MVC)
- **Lista de Empleados (`th:each`):** `http://13.140.209.186:8085/detalles_info`
![Lista](img/lista.png)
- **Formulario de Registro (`@ModelAttribute`):** `http://13.140.209.186:8085/form` *(Envía datos por POST a `/guardar`)*
![Lista](img/form.png)
### 2. Endpoints REST (JSON)
- **DTO:** `http://13.140.209.186:8085/api/detalles_info2`
![Lista](img/dto.png)
- **Query Parameters (`@RequestParam`):**
  * Detalle: `http://13.140.209.186:8085/api/parametros/detalle?informacion=TextoPrueba`
  ![Lista](img/detalle.png)
  * Saludo: `http://13.140.209.186:8085/api/parametros/saludo?nombre=Jorge`
  ![Lista](img/saludo.png)
- **Path Variables (`@PathVariable`):**
  * Mensaje: `http://13.140.209.186:8085/api/variable/pagina1/MiMensaje`
  ![Lista](img/mensajes.png)
  * ID Empleado: `http://13.140.209.186:8085/api/variable/empleado/1`
  
- **Propiedades personalizadas (`@Value`):** `http://13.140.209.186:8085/api/variable/valores`
![Lista](img/consulta.png)
- **Petición POST (`@RequestBody`):** `http://13.140.209.186:8085/api/variable/solicitud` *(Probar en Postman/Bruno enviando un JSON de Empleado)*
![Lista](img/postman.png)


- **Instancia Activa:** `http://13.140.209.186:8085/mi-instancia`