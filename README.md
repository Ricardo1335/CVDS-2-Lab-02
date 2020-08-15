# CVDS-2-Lab-02

## La herramienta Maven

1. **Ingresar a la página de la herramienta y entender:**
	+ **Cuál es su mayor utilidad:** La mayor utilidad de Maven es simplificar el proceso de construcción de proyectos de software basándose en el concepto de Project Object Model (POM). Maven administra la construcción de un proyecto a partir de una pieza central de información. 
	+ **Fases de Maven:** 
		+ **validar:** se valida que el proyecto es correcto y que toda la información necesaria está disponible.
		+ **compilar:** compilar el código fuente del proyecto.
		+ **probar:** testear el código compilado usando   
un marco de prueba unitario adecuado. Estos tests no deberían necesitar que el codigo esté empacado.
		+ **empacar:** tomar el código compilado y empacarlo en un formato distribuible como un JAR.
		+ **test de integración:** procesar e implementar el paquete si es necesario en un entorno donde se puedan ejecutar pruebas de integración.
		+ **verificar:** ejecutar cualquier verificación para verificar que el paquete sea válido y cumpla con los criterios de calidad
		+ **instalar:** instala el paquete en el repositorio local, para usarlo como dependencia en otros proyectos localmente.
		+ **desplegar:** hecho en un entorno de integración o lanzamiento, copia el paquete final en el repositorio remoto para compartirlo con otros desarrolladores y proyectos.
		+ **limpiar:** limpia los artefactos creados por compilaciones anteriores.
		+ **sitio:** genera documentación del sitio para este proyecto. 
	+ **Ciclo de vida de la construcción:** Hay tres ciclos de vida de compilación integrados: predeterminado, limpio y de sitio. El defaultciclo de vida maneja la implementación del proyecto, el cleanciclo de vida maneja la limpieza del proyecto, mientras que el siteciclo de vida maneja la creación de la documentación del sitio de su proyecto.
	+ **Para qué sirven los plugins:** Los plugins son la característica central de Maven que permiten la reutilización de la lógica de compilación común en múltiples proyectos. Los plugins se utilizan para: crear archivos jar, crear archivos war, compilar código, código de prueba unitaria, crear documentación de proyecto, etc.
	+ **Qué es y para qué sirve el repositorio central de maven:** El repositorio central de Maven es un sitio web donde se guardan todos los archivos Java. Puede buscar los jars que necesita allí. Cuando busque los archivos jar necesarios, puede incluir los archivos jar usando pom.xml o descargar directamente los archivos jar y agregarlos a su proyecto java.