
🎬 ScreenMatch Frases - Alura LATAM
Proyecto realizado como parte del desafío de Alura LATAM, en el cual se desarrolló una aplicación web que muestra frases célebres de series y películas. La aplicación está compuesta por un backend en Java con Spring Boot y un frontend en HTML, CSS y JavaScript, consumiendo una API REST y utilizando PostgreSQL como base de datos.

📂 Estructura del proyecto
🛠 Backend (Spring Boot)
El backend sigue una arquitectura MVC organizada en los siguientes paquetes:

model: contiene la entidad Frase.

repository: incluye FraseRepository, una interfaz que extiende JpaRepository.

service: contiene la lógica de negocio, como FraseService.

dto: define FraseDTO para transferencia de datos.

controller: expone los endpoints REST.

config: configuración de la base de datos y otros elementos de Spring.

🔗 Endpoint principal expuesto:
GET /series/frases

Devuelve una frase aleatoria de una serie o película.

🖥 Frontend (HTML + JS)
El frontend es una página que carga dinámicamente una frase usando JavaScript.

Archivos principales:

index.html: estructura de la página.

index.js: se encarga de cargar la frase al iniciar y al hacer clic en "Ver otras frases...".

getDatos.js: módulo para realizar peticiones al backend.

📸 Se muestra:

Imagen del poster.

Frase icónica.

Nombre del personaje que la dice.

Título de la serie/película.

🛢 Base de datos
Se utiliza PostgreSQL para almacenar las frases. La configuración debe estar en el archivo application.properties o application.yml en el backend, apuntando a tu base local/remota de PostgreSQL.

Ejemplo:
spring.datasource.url=jdbc:postgresql://localhost:5432/screentmatch
spring.datasource.username=tu_usuario
spring.datasource.password=tu_contraseña

▶️ ¿Cómo ejecutar?
Clona el repositorio:
git clone https://github.com/ivanfr12/Screenmatch-frases
cd screenmatch-frases

Configura PostgreSQL: crea la base de datos y asegúrate de que la conexión está definida correctamente en el backend.

Ejecuta el backend (Java + Spring Boot):
./mvnw spring-boot:run

Abre el index.html en tu navegador: no requiere servidor adicional, solo asegúrate que el backend esté corriendo en http://localhost:8080.

💡 Funcionalidades
Consulta aleatoria de frases famosas.

Interfaz simple y responsiva.

Código modular y separado en capas.

👨‍💻 Tecnologías usadas
Java 17 + Spring Boot

PostgreSQL

HTML5 + CSS + JavaScript (ES6 Modules)

Fetch API para el consumo del backend

📸 Vista previa
![image](https://github.com/user-attachments/assets/1902e4d4-b375-42c2-932f-8f56ab4bbddf)

