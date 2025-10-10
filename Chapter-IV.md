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
Para el desarrollo de Chapa Tu Ruta, se han adoptado las siguientes guías de estilo y convenciones de codificación para
asegurar la consistencia y calidad del código en todo el proyecto:<br>
**HTML**<br>
Durante el desarrollo en HTML se aplicaron las Convenciones de Codificación establecidas para este lenguaje, integrando 
además el uso del framework Vue junto con Vite para optimizar el rendimiento y la organización del proyecto. 
Los aspectos más relevantes implementados son:

* Empleo de etiquetas semánticas: Se utilizaron elementos como header, nav, main y footer con el propósito de mejorar 
la accesibilidad, la estructura y la comprensión del contenido del documento.

* Estructura e indentación: Aunque HTML permite el uso indistinto de mayúsculas y minúsculas en los nombres de etiquetas
y atributos, se decidió emplear únicamente minúsculas para mantener la claridad y uniformidad del código. Asimismo, 
se adoptó la convención kebab-case para garantizar coherencia en la nomenclatura y facilitar el mantenimiento del proyecto.

**CSS**<br>
**CSS**

En el desarrollo de los estilos se siguieron las **convenciones BEM** y las **guías de estilo recomendadas**, con el propósito de mantener un código estructurado, legible y fácil de mantener. Además, se emplearon **variables personalizadas en `:root`** para definir la paleta de colores y las transiciones del sitio, lo que permite una gestión más eficiente del diseño y facilita futuras modificaciones.

### Principales características implementadas

- **Uso de variables CSS personalizadas:**  
  En el selector `:root` se declararon múltiples variables (`--cl-orange`, `--cl-purple`, `--cl-green`, etc.) para estandarizar la paleta de colores y asegurar coherencia visual en toda la interfaz.

- **Compatibilidad con modo claro y oscuro:**  
  Se utilizó la regla `@media (prefers-color-scheme: light)` para ajustar automáticamente los colores del sitio según la preferencia del usuario, mejorando la accesibilidad y experiencia visual.

- **Tipografía y legibilidad:**  
  Se definió una jerarquía tipográfica clara empleando fuentes del sistema y ajustes de renderizado (`-webkit-font-smoothing`, `-moz-osx-font-smoothing`) para optimizar la legibilidad en diferentes dispositivos.

- **Diseño responsivo:**  
  Se incluyeron márgenes dinámicos (`--sideMargin`, `--sideMarginMobile`) y transiciones suaves (`--n-out`, `--n-in-out`) para adaptar el contenido a distintos tamaños de pantalla, manteniendo una apariencia consistente.

- **Transiciones y efectos interactivos:**  
  Los botones (`button`) cuentan con **transiciones suaves y efectos hover**, aportando dinamismo y una mejor experiencia de usuario.

En conjunto, este enfoque garantiza un diseño moderno, coherente y adaptable, alineado con las buenas prácticas de desarrollo frontend.

**JavaScript**

Para la parte funcional del proyecto se utilizó **JavaScript** junto con el **framework Vue 3** y el **empaquetador Vite**, lo que permitió un desarrollo modular, rápido y eficiente.  
El código principal inicializa la aplicación, configura dependencias y registra los componentes visuales.

### Principales características implementadas

- **Inicialización del proyecto con Vue 3:**  
  La aplicación se crea mediante la función `createApp(App)`, que establece la estructura base del proyecto y monta la interfaz en el elemento raíz identificado como `#app`.

- **Integración del framework PrimeVue:**  
  Se incorporó **PrimeVue** como biblioteca principal de componentes UI, configurada con el **tema Aura** para garantizar una estética moderna y coherente.  
  La personalización del tema se definió a través de opciones como `prefix`, `darkModeSelector` y `cssLayer`, adaptando la integración al diseño del sitio.

- **Internacionalización (i18n):**  
  Se implementó el módulo `i18n.js` para manejar la **traducción de contenidos** entre diferentes idiomas, optimizando la experiencia del usuario en contextos multilingües.

- **Registro de componentes globales:**  
  Los componentes `Button` y `SelectButton` de PrimeVue fueron registrados globalmente bajo los nombres `pb-Button` y `pb-SelectButton`, facilitando su reutilización en distintas secciones del proyecto.

- **Importación modular de estilos:**  
  Los estilos globales se administran a través del archivo `style.css`, que se integra en la aplicación para mantener la coherencia visual junto con las configuraciones de tema y tipografía.

En conjunto, este enfoque permite mantener un código **escalable, limpio y orientado a componentes**, alineado con las mejores prácticas de desarrollo frontend moderno.

**Kotlin (Android Studio)**

En el desarrollo de la aplicación móvil se siguieron las directrices de la **Google Kotlin Style Guide**, con el objetivo de mantener un código limpio, coherente y fácil de mantener dentro del entorno de **Android Studio**.

### Principales características implementadas

- **Convenciones de nomenclatura:**  
  Se aplicó la convención **PascalCase** para la definición de clases y métodos, mientras que los atributos y variables de instancia se nombraron utilizando **lowerCamelCase**, garantizando uniformidad y legibilidad en todo el código.

- **Estructura y organización del proyecto:**  
  El proyecto se diseñó bajo la metodología de **Clean Architecture**, complementada con los principios de **Domain Driven Design (DDD)**.  
  La estructura se organizó en **Bounded Contexts**, y cada uno de ellos se dividió en capas bien definidas, tales como **Repositorios**, **Casos de Uso**, **Dominios** y **UI**, lo que favorece la separación de responsabilidades y la escalabilidad del sistema.

En conjunto, estas prácticas permiten mantener una arquitectura sólida, modular y alineada con las mejores prácticas de desarrollo en Kotlin para Android.

### 4.1.4.Software Deployment Configuration
**Landing Page**

Para el despliegue de la **Landing Page**, se utilizó **GitHub Pages**, la funcionalidad integrada de GitHub que permite publicar sitios web estáticos de manera sencilla y gratuita.

### Proceso de implementación

- **Creación del repositorio:**  
  Desde la cuenta de GitHub, se seleccionó la opción **"New Repository"** para crear un nuevo repositorio donde se alojará el proyecto.

- **Configuración del repositorio:**  
  Se asignó un nombre identificativo al repositorio y se configuró con visibilidad **pública**, requisito necesario para que GitHub Pages pueda realizar el despliegue del sitio.

**Configuración del despliegue con GitHub Pages**

Para proceder con el despliegue de la **Landing Page**, se creó una nueva rama denominada `feature/chapter-IV-deployment`, con el objetivo de mantener aislados los cambios relacionados con la configuración del entorno de publicación.  
A continuación, se ejecutó el comando `git branch` para verificar las ramas activas en el repositorio, confirmando que la rama actual de trabajo era la recién creada.

Posteriormente, se instaló el paquete **gh-pages** mediante el siguiente comando:

```bash
npm install gh-pages --save-dev
```
![img_1.png](img_1.png)

**Ejecución del despliegue**

Una vez instalada la dependencia **gh-pages** y configurado el script de despliegue en el archivo `package.json`, se procedió a ejecutar el comando:

```bash
npm run deploy
```
![img_2.png](img_2.png)
**Configuración de github Pages**

Una vez ejecutado el despliegue con `npm run deploy`, el sitio quedó alojado en la rama **`gh-pages`** del repositorio.  
Para finalizar la configuración, se accedió a la pestaña **Settings → Pages** dentro del repositorio de GitHub.

### Detalles de la configuración

- **Fuente de despliegue (Source):**  
  Se seleccionó la opción **"Deploy from a branch"**, indicando que el sitio será publicado directamente desde una rama del repositorio.

- **Rama de publicación (Branch):**  
  Se estableció la rama **`gh-pages`** como la fuente del sitio, con el directorio raíz **`/(root)`**, lo que permite a GitHub Pages leer directamente los archivos estáticos generados en la carpeta `dist` durante el proceso de build.

- **URL del sitio:**  
  GitHub genera automáticamente la URL de acceso público:  
  👉 [https://aplicaciones-moviles-grupo.github.io/landing-page-original/](https://aplicaciones-moviles-grupo.github.io/landing-page-original/)

Esta configuración asegura que la **Landing Page** se mantenga disponible en línea y que cualquier actualización futura en el código pueda desplegarse fácilmente con un nuevo `npm run deploy`.

![img_3.png](img_3.png)


## 4.2.Landing Page & Mobile Application Implementation

### 4.2.1.Sprint 1

#### 4.2.1.1.Sprint Planning 1

#### 4.2.1.2.Sprint Backlog 1

#### 4.2.1.3.Development Evidence for Sprint Review

**LANDING PAGE**<br>
En el desarrollo de la **Landing Page**, la implementación estuvo a cargo de un único integrante del equipo.  
Por esta razón, el proyecto se trabajó **exclusivamente en su entorno local**, sin requerir colaboración simultánea en línea.  
Esta decisión se tomó por **comodidad y eficiencia**, dado que el alcance del proyecto era reducido y no implicaba la necesidad de integración con otros desarrolladores.

Posteriormente, el proyecto fue desplegado en **GitHub Pages** para su publicación, permitiendo que el resto del equipo y los evaluadores pudieran visualizar la versión final directamente desde la web.

<table><thead>
  <tr>
    <th>&nbsp;&nbsp;&nbsp;<br>Repository&nbsp;&nbsp;&nbsp;</th>
    <th>&nbsp;&nbsp;&nbsp;<br>Branch&nbsp;&nbsp;&nbsp;</th>
    <th>&nbsp;&nbsp;&nbsp;<br>Commit ID&nbsp;&nbsp;&nbsp;</th>
    <th>&nbsp;&nbsp;&nbsp;<br>Commit<br>&nbsp;&nbsp;&nbsp;<br>Message&nbsp;&nbsp;&nbsp;</th>
    <th>&nbsp;&nbsp;&nbsp;<br>Commit<br>&nbsp;&nbsp;&nbsp;<br>Message Body&nbsp;&nbsp;&nbsp;</th>
    <th>&nbsp;&nbsp;&nbsp;<br>Committed on&nbsp;&nbsp;&nbsp;(Date)&nbsp;&nbsp;&nbsp;</th>
  </tr></thead>
<tbody>
  <tr>
<td rowspan="10">
	<h5>Landing Page</h5>
	<a href="https://aplicaciones-moviles-grupo.github.io/landing-page-original" target="_blank" rel="noopener noreferrer">https://aplicaciones-moviles-grupo.github.io/landing-page-original</a>
	<br>
</td>
    <td><br>main</td>
    <td><br>9d66d7fd7ccd87ec117c25cb8dcc7bb561dad065</td>
    <td><br>first commit</td>
    <td><br>first commit</td>
    <td><br>Oct 8, 10:38 PM GMT-5</td>
  </tr>
</tbody></table>

**BACKEND**<br>
<table><thead>
  <tr>
    <th>&nbsp;&nbsp;&nbsp;<br>Repository&nbsp;&nbsp;&nbsp;</th>
    <th>&nbsp;&nbsp;&nbsp;<br>Branch&nbsp;&nbsp;&nbsp;</th>
    <th>&nbsp;&nbsp;&nbsp;<br>Commit ID&nbsp;&nbsp;&nbsp;</th>
    <th>&nbsp;&nbsp;&nbsp;<br>Commit<br>&nbsp;&nbsp;&nbsp;<br>Message&nbsp;&nbsp;&nbsp;</th>
    <th>&nbsp;&nbsp;&nbsp;<br>Commit<br>&nbsp;&nbsp;&nbsp;<br>Message Body&nbsp;&nbsp;&nbsp;</th>
    <th>&nbsp;&nbsp;&nbsp;<br>Committed on&nbsp;&nbsp;&nbsp;(Date)&nbsp;&nbsp;&nbsp;</th>
  </tr></thead>
<tbody>
  <tr>
    <td rowspan="10">
	    <h5>back-end</h5>
	      <a href="https://github.com/Aplicaciones-Moviles-Grupo/back-end" target="_blank" rel="noopener noreferrer">https://github.com/Aplicaciones-Moviles-Grupo/back-end</a>
	      <br>
    </td>
    <td><br>main</td>
    <td><br>fc929b77270f95aba6a35387a96a7503c3523529</td>
    <td><br>first commit</td>
    <td><br>first commit</td>
    <td><br>Oct 6, 2025</td>
  </tr>
 <tr>
   <td><br>main</td>
    <td><br>cf7d59caa7536a1f3aa87852fa8ef0b899349d49</td>
    <td><br>feature: update database connection settings for production environment</td>
    <td><br>feature: update database connection settings for production environment</td>
    <td><br>Oct 8, 2025</td>
  </tr>
</tbody></table>

#### 4.2.1.4.Testing Suite Evidence for Sprint Review

En este **Sprint**, se presentarán los archivos con extensión **`.feature`**, los cuales documentan los **user tasks** desarrollados durante esta etapa.  
Estos archivos siguen el formato **Gherkin**, utilizado para describir de forma clara y estructurada los escenarios de comportamiento esperados del sistema.

Cada `.feature` corresponde a una funcionalidad o historia de usuario implementada, e incluye sus respectivos escenarios y criterios de aceptación.  
Todos los archivos han sido **subidos al repositorio del proyecto**, donde pueden consultarse para revisar el avance, validación y trazabilidad de los requerimientos implementados.


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

**Evidencias del despliegue de la Landing Page**

A continuación, se presentan las evidencias del **despliegue de la Landing Page**, desarrollada con **Vue 3**, **Vite** y **JavaScript**.  
El proyecto fue construido aplicando componentes dinámicos y estilos personalizados, y posteriormente publicado mediante la funcionalidad de **GitHub Pages**, la cual permite alojar sitios web estáticos directamente desde un repositorio.

Durante el proceso se generó la carpeta `dist/` con los archivos optimizados para producción, y se configuró el despliegue automático hacia la rama `gh-pages`.  
De esta manera, la página quedó disponible públicamente, mostrando la integración entre **Vue**, **Vite** y las configuraciones de despliegue en **GitHub Pages**.

**url:** <a href="https://aplicaciones-moviles-grupo.github.io/landing-page-original">https://aplicaciones-moviles-grupo.github.io/landing-page-original</a>


![img_4.png](img_4.png)
**Como trabajamos**<br>
![img_5.png](img_5.png)
![img_6.png](img_6.png)
![img_7.png](img_7.png)

**Evidencias del despliegue del Back End**<br>
**Despliegue del Web Service**

Para el **despliegue del Web Service**, se utilizó la plataforma **Railway**, la cual se integró directamente con el repositorio de **GitHub**.  
Esta conexión permitió automatizar el proceso de despliegue, de modo que cada cambio o actualización en el código del repositorio se reflejara automáticamente en el entorno en línea.

Railway ofrece una configuración sencilla y flexible, ideal para proyectos con backend ligero o servicios web basados en APIs.  
A través de su panel, se vinculó el repositorio del proyecto, se configuraron las variables de entorno necesarias y se ejecutó el despliegue con un solo clic, sin necesidad de herramientas externas o autenticaciones adicionales desde el IDE.

![img_8.png](img_8.png)

**Actualización del despliegue en Railway**

En la imagen se muestra el panel de control de **Railway**, donde se registran los cambios aplicados al proyecto del **Web Service**.  
El sistema indica que se realizaron **dos actualizaciones** relacionadas con la configuración del entorno de despliegue:

- **Branch:**  
  Se confirma que la rama activa para el despliegue es `main`, lo que significa que Railway tomará automáticamente el código más reciente de esta rama cada vez que se realice un nuevo commit o push en GitHub.

- **Repo:**  
  Se muestra el repositorio vinculado al servicio, en este caso **`Aplicaciones-Moviles-Grupo/back-end`**, el cual contiene el código fuente del backend.

El mensaje **“back-end was updated”** confirma que Railway detectó cambios en el repositorio y actualizó el entorno de producción de forma automática.  
Esta funcionalidad garantiza una **integración continua** entre GitHub y Railway, permitiendo que cada modificación validada en la rama principal se despliegue sin intervención manual adicional. 
![img_9.png](img_9.png)

**Evidencia de despliegue en Railway**

La imagen muestra el entorno de **producción** en **Railway**, donde el **backend** fue desplegado correctamente.

- **Estado:** El mensaje *“Deployment successful”* confirma que el despliegue se realizó sin errores.
- **Origen:** El código se obtuvo automáticamente desde la rama `main` del repositorio **`Aplicaciones-Moviles-Grupo/back-end`**, mediante integración con **GitHub**.
- **Configuración:** El servicio usa un **Dockerfile** para su construcción y ejecuta el comando `./Frock-backend` al iniciar.

Con esto se valida que el **Web Service** se encuentra activo y funcionando en producción con un flujo automatizado de despliegue continuo.
![img_10.png](img_10.png)

**Despliegue del Web Service en Railway**

finalmente, se muestra la URL pública generada por **Railway** para acceder al **Web Service** desplegado.
![img_11.png](img_11.png)

#### 4.2.1.8.Team Collaboration Insights during Sprint
