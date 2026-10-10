Prueba de automatización
✅ Prerrequisitos
Asegúrate de tener las siguientes herramientas y versiones instaladas en tu máquina local con Windows 10:

IDE IntelliJ IDEA versión 2023.1 o superior
Apache Maven versión 3.9.8 (debe estar configurado en la variable de entorno PATH)
JDK versión 25 LTS (debe estar configurado en la variable de entorno JAVA_HOME)


📦 Comandos de instalación
Para configurar tu entorno de desarrollo, sigue estos pasos:


Clonar el repositorio:
Shellgit clone https://github.com/MaribelDS/ApiKarateDemoglazeMostrar más líneas


Compilar el proyecto:

Ejecuta el siguiente comando para descargar todas las dependencias del pom.xml:
Shellmvn install -DskipTestsMostrar más líneas

O desde IntelliJ IDEA, ve al panel derecho → MAVEN → clic en Reload all maven projects




🧪 Instrucciones para ejecutar los tests
Desde IntelliJ IDEA

Abre el proyecto en IntelliJ IDEA.
Configura el entorno de ejecución para ejecutar los tests de Karate.
Dirígete al archivo:
src/test/resources/demoblaze.feature


Ejecuta el archivo directamente desde el IDE.

Desde Maven
Ejecuta el siguiente comando en la terminal dentro del directorio raíz del proyecto:
Shellmvn testMostrar más líneas
Esto iniciará la ejecución de todos los tests definidos en el proyecto.

📊 Reporte
Al ejecutar los tests, se genera un reporte con evidencias por cada paso del escenario Gherkin. Este se encuentra en:
target/karate-reports/karate-summary.html

Al finalizar la ejecución, se muestra en consola el path del reporte. Puedes hacer Ctrl + Click sobre ese path para abrirlo directamente en tu navegador.

📁 Estructura del proyecto
Las evidencias generadas se almacenan en la carpeta evidencias/, de acuerdo con la siguiente estructura del proyecto:
pom.xml
README.md
conclusiones_demoblaze_API.txt
.idea/
target/
evidencias/
src/


⚠️ Observaciones

Al realizar el signup de la API en Karate, se refleja un mensaje de error distinto al esperado.
Sin embargo, al realizar el mismo proceso desde la web de Demoblaze, el mensaje es el correcto.
