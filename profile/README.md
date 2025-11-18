<p align="center">
    <img width="200" height="200" alt="Logo Argy" src="https://github.com/user-attachments/assets/49bc4773-13c1-49ca-8acc-7a5745c02674" />
</p>
<!--horizontal divider(gradiant)-->
<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif">
<p align="center">
 <a href="https://git.io/typing-svg">
</p>

## Nostros somos los integrantes de Argy Spot:

 | <a href="https://github.com/sharly-dev"><img src="https://avatars.githubusercontent.com/u/155045111?v=4" width="200"></a> | <a href="https://github.com/silvag-daniels"><img src="https://avatars.githubusercontent.com/u/178740893?v=4" width="200"></a> | <a href="https://github.com/ejgonzalez16"><img src="https://avatars.githubusercontent.com/u/169292875?v=4" width="200"></a> | <a href="https://github.com/majo425"><img src="https://github.com/user-attachments/assets/f80d1618-66c1-4854-9d4a-7e5b5e660ec6" width="200"></a> |
|:--:|:--:|:--:|:--:|
[**Carlos Andrés Carrero Sandoval**](https://github.com/sharly-dev) | [**Daniel Santiago Silva Gomez**](https://github.com/silvag-daniels) | [**Édgar Julián González Sierra**](https://github.com/ejgonzalez16) | [**María José Cárdenas Machaca**](https://github.com/majo425)


<h3> Indice: </h3>

- [📖 Descripción](#-descripción)
- [⚙️ Servicios y hardware utilizados](#%EF%B8%8F-servicios-y-hardware-utilizados)
- [💬 ​DCU (Diagrama de Casos de Uso)](#-dcu-diagrama-de-casos-de-uso)
- [📦 DC (Diagrama de Clases)](#-dc-diagrama-de-clases)
- [🎨 Pantallas principales de la aplicación (mockups)](#-pantallas-principales-de-la-aplicación-mockups)


<!--horizontal divider(gradiant)-->
<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif">

<h3>📖 Descripción</h3>

Argy Spot es un sistema el cual se accede a través de una aplicación móvil, el cual ofrece las funcionalidades que permite recomendar, demostrar, corregir y cuantificar los ejercicios de fuerza. Pues se permite hacer recomendaciones y crear preferencias de usuario a partir de un LLM, mostrar la correcta ejecución de los ejercicios a través de realidad aumentada, corregir los rangos articulares del usuario en la ejecución y mostrar estadísticas acerca de los ejercicios realizados.

<h3>⚙️ Servicios, hardware y repositorios utilizados</h3>

- **📱 Aplicación móvil Android**
  - Todas las funcionalidades del sistema se utilizan a través de la aplicación Android.
  
- **📷 Uso de la Cámara**
  - Se hace uso de la cámara para mostrar las animaciones 3D en realidad aumentada y corregir la ejecución del usuario en tiempo real.

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

- **🖥️ Docker Compose**
  - 



<h3>💬 ​DCU (Diagrama de Casos de Uso)</h3>

<p align="center">
    <img width="1000" src="https://github.com/user-attachments/assets/114f5ecf-bc6b-4cb1-84aa-ee8c87b278af">
</p>

<h3>📦 DC (Diagrama de Despliegue)</h3>

<p align="center">
    <img width="1000" src="https://github.com/user-attachments/assets/1af55061-24e3-48a2-a4e4-a8612f427d15">
</p>

