# Capítulo IV: Product Implementation & Validation

## 4.1.Software Configuration Management

### 4.1.1.Software Development Environment Configuration

Para asegurar una colaboración eficiente y mantener la calidad en el desarrollo de **Chapa Tu Ruta**, se ha definido un entorno de desarrollo común para todos los miembros del equipo. A continuación, se listan los productos de software utilizados en las distintas etapas del ciclo de vida del producto digital, indicando su propósito y su enlace de referencia o descarga correspondiente.

**Product UX/UI Design**

Para el diseño de la experiencia de usuario y la interfaz de la Landing page de Eventify, se utilizaron las siguientes herramientas:

- Figma: Se empleó para la creación de wireframes, mock-ups y prototipos de la aplicación web.[https://www.figma.com/es-es/](https://www.figma.com/es-es/)
- UXPressia: Utilizada para elaborar User Personas, Empathy Maps, Journey Maps e Impact Maps. [https://uxpressia.com/](https://uxpressia.com/)
- Miro: Se utilizó para la creación de Event Storming, Domain Message Flow Modelling, Bounded Context Canvases. [https://miro.com/es/](https://miro.com/es/)

**Software Development**

Para el desarrollo del software del Landing Page, Backend y Mobile App, se adoptaron los siguientes productos:

- WebStorm (Instalación local): Utilizado como entorno de desarrollo para trabajar con HTML, CSS y JavaScript. [https://www.jetbrains.com/es-es/webstorm/](https://www.jetbrains.com/es-es/webstorm/)
- Android Studio (Instalación local): Este es un IDE para desarrollar aplicaciones móviles para Android, utilizando Kotlin y JetPack Compose. [https://developer.android.com/studio?hl=es-419](https://developer.android.com/studio?hl=es-419)
- Rider(Instalación local): Utilizamos este IDE para desarrollar el backend de la aplicación. [https://www.jetbrains.com/es-es/rider](https://www.jetbrains.com/es-es/rider)
- Git (Instalación local): Empleado para gestionar los cambios de código de manera local mediante commits y ramas. [https://git-scm.com/](https://git-scm.com/)
- GitHub: Plataforma de repositorio remoto para la gestión de versiones del código, implementando el flujo GitFlow para garantizar un desarrollo organizado. [https://github.com/](https://github.com/)

**Project Management and Collaboration**

En la gestión de proyectos y colaboración del equipo se utilizaron:

- **Trello:** Utilizado para la planificación y seguimiento de tareas, distribuidas en listas de "por hacer", "en progreso" y "hecho".
- **WhatsApp:** Medio de comunicación instantánea para coordinar avances, resolver dudas rápidas y hacer recordatorios. [https://web.whatsapp.com/](https://web.whatsapp.com/)
- **Google Meet:** Herramienta utilizada para realizar reuniones virtuales más formales, presentaciones de avances y coordinación general del equipo. [https://www.zoom.com/es](https://www.zoom.com/es)

**Software Documentation**

Para la documentación del proyecto se emplearon las siguientes herramientas:
 
- Lucidchart: Utilizada para la creación de diagramas UML, wireflows y user flows que ayudan en la planificación y visualización del sistema. [https://www.lucidchart.com/pages](https://www.lucidchart.com/pages)
- Visual Paradigm: Herramienta usada para modelar la arquitectura de software mediante diagramas C4. [https://online.visual-paradigm.com/drive/#proj=0&dashboard](https://online.visual-paradigm.com/drive/#proj=0&dashboard)


### 4.1.2.Source Code Management

La gestión del código fuente es una parte fundamental en el desarrollo colaborativo de software, ya que permite un control eficiente sobre las modificaciones realizadas en el proyecto a lo largo de su ciclo de vida. En esta sección del informe, se describe el sistema de control de versiones implementado en el proyecto Chapa Tu Ruta, utilizando GitHub como plataforma principal. Además, se detallan las convenciones de trabajo adoptadas por el equipo, como el modelo GitFlow, el versionado semántico (Semantic Versioning) y las convenciones de commit mediante Conventional Commits. Estas prácticas aseguran un desarrollo ordenado y una integración continua efectiva entre los miembros del equipo.

**URL de los Repositorios:**
- Organización: [https://github.com/Aplicaciones-Moviles-Grupo](https://github.com/Aplicaciones-Moviles-Grupo)
- Reporte: [https://github.com/Aplicaciones-Moviles-Grupo/Report](https://github.com/Aplicaciones-Moviles-Grupo/Report)
- Landing Page: [https://github.com/Aplicaciones-Moviles-Grupo/landing-page-original](https://github.com/Aplicaciones-Moviles-Grupo/landing-page-original)
- Backend: [https://github.com/Aplicaciones-Moviles-Grupo/back-end](https://github.com/Aplicaciones-Moviles-Grupo/back-end)
- Aplicación Movil: [https://github.com/Aplicaciones-Moviles-Grupo/ChapaTuRuta-MobileApp](https://github.com/Aplicaciones-Moviles-Grupo/ChapaTuRuta-MobileApp)

**Estructura de Ramas:**

Para mantener un flujo organizado en el desarrollo y facilitar la colaboración, se ha implementado el modelo GitFlow, creando las siguientes ramas:

- Main Branch: Rama principal (main) que contiene las versiones estables del proyecto. Todas las demás ramas derivan de esta.
- Develop: Rama secundaria donde se integran todas las características nuevas antes de fusionarse a la rama main.
- Feature Branches: Estas ramas se crean a partir de develop y son en base a las características del proyecto. Una vez se termina de trabajar en la rama, se hace merge hacia develop.

**Convenciones de commits:**

Para la escritura de commits en el proyecto Eventify, se sigue la convencion 'Conventional Commits', el cual cuenta con un formato estándar para facilitar la lectura y entendimiento del historial de cambios dentro del proyecto.
```
    <type>[optional scope]: <description>
    
    [optional body]
    
    [optional footer(s)]
```
- Type:
    - feat: Añadir una nueva característica.
    - fix: Correción de errores.
    - docs: Modificaciones en la documentación.
    - style: Cambios que no afectan la lógica del código.
    - refactor: Modificaciones que no añaden características y/o errores.
    - test: Adición/Modificación de pruebas.


- Scope: Brinda información extra acerca del área del codigo afectado.
```
   feat(auth): add register functionality.
```
**Ejemplos básicos de commits:**
```
   feat(login): add organizer authentication module.
```
```
   fix(payment): resolve payment security issue.
```
```
   docs(README): update index instructions.
```

### 4.1.3.Source Code Style Guide & Conventions

### 4.1.4.Software Deployment Configuration

## 4.2.Landing Page & Mobile Application Implementation

### 4.2.1.Sprint 1

#### 4.2.1.1.Sprint Planning 1

En este primer sprint, el equipo se centró en el desarrollo y mejora de la aplicación móvil “Chapa Tu Ruta” en Android Studio.  
El objetivo principal fue implementar las principales vistas funcionales y establecer la navegación entre ellas.  

Las tareas se distribuyeron de la siguiente manera:

- **Adrián Valerio**: Implementación de las vistas de **Login** y **Registro de usuario** (RegisterUserView y RegisterProfileView), además de la configuración del **AppNavHost** para gestionar la navegación.
- **Yasser Renteria**: Desarrollo de la **pantalla de creación de rutas**, enfocada en permitir al conductor o usuario registrar rutas personalizadas dentro de la app móvil.
- **Renzo Araujo**: Implementación de la **página de edición de perfil**, donde los usuarios pueden actualizar sus datos personales y de vehículo.
- **Fabrizio Cutiri**: Creación de la **página principal (Home)** que sirve como punto de inicio después del inicio de sesión, mostrando las rutas y accesos a las demás funcionalidades.

También se añadió el **logo oficial de la aplicación** en todas las vistas principales para unificar la identidad visual.

#### 4.2.1.2.Sprint Backlog 1

| ID | Historia de Usuario | Descripción | Prioridad | Responsable | Estado |
|----|----------------------|-------------|------------|--------------|---------|
| HU-01 | Inicio de Sesión | Como usuario, quiero iniciar sesión con mis credenciales para acceder a la app. | Alta | Adrián | Completado |
| HU-02 | Registro de Usuario | Como nuevo usuario, quiero registrarme ingresando mis datos personales y del vehículo. | Alta | Adrián | Completado |
| HU-03 | Crear Ruta | Como conductor, quiero registrar rutas para ofrecer mis servicios. | Media | Yasser | En desarrollo |
| HU-04 | Editar Perfil | Como usuario, quiero editar mi información personal para mantenerla actualizada. | Media | Renzo | Completado |
| HU-05 | Página Principal (Home) | Como usuario, quiero acceder a la pantalla principal después del login para ver y navegar entre secciones. | Alta | Fabrizio | Completado |
| HU-06 | Navegación entre pantallas | Implementar navegación entre Login, Registro, Perfil, Home y Crear Ruta. | Alta | Adrián | Completado |
| HU-07 | Integrar logo institucional | Añadir el logo oficial de la app en todas las vistas principales. | Media | Todo el equipo | Completado |

#### 4.2.1.3.Development Evidence for Sprint Review

#### 4.2.1.4.Testing Suite Evidence for Sprint Review

#### 4.2.1.5.Execution Evidence for Sprint Review

Durante este primer Sprint logramos realizar la implementación del Landing page, Backend y Mobile App, sin embargo este último por el momento se realizó de forma local.

A continuación se presentan evidencias de ejecución de los 3 productos:


**Landing Page**

**Hero Section**: En esta sección se colocó un mensaje que atraiga la atención del visitante, junto con un boton call to action para posteriormente enviarlo a la aplicación movil desplegada. 

<img src="resources/chapter-4/Hero%20Section.png" height=400>

**How It Works Section**: En esta sección se le presenta como funciona la app para que el usuario obtenga información sobre las rutas y paraderos de los colectivos 

<img src="resources/chapter-4/How-it-Work.png" height=400>

**Advantages Section**: Se presentan los beneficios que ofrece la aplicación para facilitar la búsqueda de colectivos

<img src="resources/chapter-4/Advantages%20Section.png" height=400>

**FAQ Section**: Se muestran las preguntas frecuentes que realizan los visitantes cuando visitan por primera vez la página

<img src="resources/chapter-4/FAQ%20Section.png" height=400>

**Footer Section**: Finalmente en el footer se presenta información de contacto como redes sociales, numero de telefono, etc.

<img src="resources/chapter-4/Footer%20Section.png" height=400>


**Backend**

<img src="resources/chapter-4/Backend-Execution-1.png" height=400>

<img src="resources/chapter-4/Backend-Execution-2.png" height=400>

<img src="resources/chapter-4/Backend-Execution-3.png" height=400>

<img src="resources/chapter-4/Backend-Execution-4.png" height=400>

<img src="resources/chapter-4/Backend-Execution-5.png" height=400>

**Mobile App**

<img src="resources/chapter-4/Mobile-App-Execution-1.png" height=400>

<img src="resources/chapter-4/Mobile-App-Execution-2.png" height=400>

<img src="resources/chapter-4/Mobile-App-Execution-3.png" height=400>

<img src="resources/chapter-4/Mobile-App-Execution-4.png" height=400>



#### 4.2.1.6.Services Documentation Evidence for Sprint Review

#### 4.2.1.7.Software Deployment Evidence for Sprint Review

#### 4.2.1.8.Team Collaboration Insights during Sprint
