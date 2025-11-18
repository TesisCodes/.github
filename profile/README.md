<p align="center">
    <img width="200" height="200" alt="Logo Argy" src="https://github.com/user-attachments/assets/49bc4773-13c1-49ca-8acc-7a5745c02674" />
</p>

## Nostros somos los integrantes de Argy Spot:

 | <a href="https://github.com/sharly-dev"><img src="https://avatars.githubusercontent.com/u/155045111?v=4" width="200"></a> | <a href="https://github.com/silvag-daniels"><img src="https://avatars.githubusercontent.com/u/178740893?v=4" width="200"></a> | <a href="https://github.com/ejgonzalez16"><img src="https://avatars.githubusercontent.com/u/169292875?v=4" width="200"></a> | <a href="https://github.com/majo425"><img src="https://github.com/user-attachments/assets/f80d1618-66c1-4854-9d4a-7e5b5e660ec6" width="200"></a> |
|:--:|:--:|:--:|:--:|
[**Carlos Andrés Carrero Sandoval**](https://github.com/sharly-dev) | [**Daniel Santiago Silva Gomez**](https://github.com/silvag-daniels) | [**Édgar Julián González Sierra**](https://github.com/ejgonzalez16) | [**María José Cárdenas Machaca**](https://github.com/majo425)


<h3> Indice: </h3>

- [📖 Descripción](#descripcion)
- [⚙️ Servicios y hardware utilizados](#servicios-hardware)
- [💬 ​Diagrama de Casos de Uso](#diagrama-de-casos-de-uso)
-  [📄 ​Diagrama de Contexto](#diagrama-contexto)
-  [📅 Diagrama de entidad relación](#diagrama-ER)
- [🔧 Diagrama de Despliegue](#diagrama-de-despliegue)


<h3 id="descripcion">📖 Descripción</h3>

Argy Spot es un sistema el cual se accede a través de una aplicación móvil, el cual ofrece las funcionalidades que permite recomendar, demostrar, corregir y cuantificar los ejercicios de fuerza. Pues se permite hacer recomendaciones y crear preferencias de usuario a partir de un LLM, mostrar la correcta ejecución de los ejercicios a través de realidad aumentada, corregir los rangos articulares del usuario en la ejecución y mostrar estadísticas acerca de los ejercicios realizados.

<h3 id="#servicios-hardware">⚙️ Servicios y tecnologías utilizadas</h3>

- **📱 Aplicación móvil Android**
  - Todas las funcionalidades del sistema se utilizan a través de la aplicación Android.

- **🌐 Nginx**
    - Reverse proxy que expone el dominio con certificado SSL y redirigir las peticiones HTTPS al Api Gateway
      
- **🔍 Eureka**
    - Servicio de registro y descubrimiento que permmite a los 6 servicios principales registrarse y darle las direcciones al Api Gateway

- **🛠️ Configuration Service**
    - Servicio de configuración centralizada en donde se aloja la configuración de los servicios desarrollados en SpringBoot
    
- **🔗 Api Gateway**
    - Encargado de obtener las direcciones a los endpoints dinámicamente del eureka y redirgir hacia el servicio en específico
     
- **👤 Servicio de autenticación**
  - Permite registrarse, hacer login y actualizar la información de usuario.
  
- **🏋🏻‍♀️ Servicio de realidad aumentada***
  - Brinda acceso a las animaciones a través de una url firmada del MinIO.
 
- **🏋️‍♀️ Servicio de ejercicios**
  - Obtiene la información de los ejercicios, las reglas y los tipos de rango.

- **📈 Servicio de estadísticas**
  - Obtiene y guarda la información de estadísticas de usuario.

- **🤖 Servicio de LLM**
  - Inserta preferencias y genera recomendaciones a partir de la información del usuario.

- **🏋️ Servicio de HPE**
  - Procesa vídeos del usuario para devolverlo con conteo de repeticiones, retroalimentación visual y auditiva, recopliación de errores y resumen de estadísticas.

- **♻️ Redis**
    - Sistema de cache que guarda los datos frecuentes del servicio de HPE.

- **🗄️ ArgyDB**
    - Base de datos MYSQL que permite guardar los datos estructurados del sistema.
 
- **🗃️ MinIO**
    - Almacenamiento de objetos, es decir almacena fotos, vídeos o animaciones que se utilicen en el sistema.

- **🛡️ Keycloak**
    - Almacena los usuarios y sus credenciales, así mismo, brinda acceso a sesiones con tokens.

- **♾️ GIT Runners**
    - Runners los cuales se conectan a los 6 repositorios de los servicios para generar el CI y CD.

- **♾️ Jenkins**
    - Contiene las tareas y credenciales necesarias para poner a funcionar el CI y CD del front.

-  **📊 Telegraf**
    - Servicio encargado de mandar las métricas de servidor a la arquitectura de pruebas.

- **📜 Exercises rules**
    - Guarda en formato json las reglas que se aplican desde la base de datos y el front.

- **🖥️ Docker Compose**
  - Encargado de desplegar toda la arquitectura del sistema en pocos pasos, incluyendo todas sus configuraciones y datos iniciales.

- **🧪 PruebasK6**
  - Código y despliegue para realizar las pruebas de carga y estrés.




<h3 id="#diagrama-de-casos-de-uso">💬 ​Diagrama de Casos de Uso</h3>

<p align="center">
    <img width="1000" src="https://github.com/user-attachments/assets/114f5ecf-bc6b-4cb1-84aa-ee8c87b278af">
</p>

<h3 id="#diagrama-contexto">📄 ​Diagrama de Contexto</h3>

<p align="center">
    <img width="1000" src="https://github.com/user-attachments/assets/873da9c5-578f-44b1-a8d7-1a86528a847f">
</p>

<h3 id="#diagrama-ER">📅 Diagrama de entidad relación</h3>

<p align="center">
    <img width="1724" height="1000" src="https://github.com/user-attachments/assets/dd29dd8b-bd9e-40d9-ac0c-91c9fe65c403" />
</p>

<h3 id="#diagrama-de-despliegue">🔧  Diagrama de Despliegue</h3>

<p align="center">
    <img width="1000" src="https://github.com/user-attachments/assets/1af55061-24e3-48a2-a4e4-a8612f427d15">
</p>

