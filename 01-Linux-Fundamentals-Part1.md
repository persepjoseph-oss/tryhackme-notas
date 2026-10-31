# Fecha: 31 de octubre de 2026 (repaso; la hice por primera vez hace unos 2 meses)

- Comandos que practiqué
- Comando	Para qué sirve
- ls  	Lista archivos y carpetas
- cd   carpeta	Entra a una carpeta
- cd ..	  Sube una carpeta
- pwd  	Muestra en qué carpeta estoy
- cat archivo	  Muestra el contenido de un archivo
- find -name archivo	  Busca archivos por su nombre
- grep "texto" archivo	  Muestra las líneas de un archivo que contienen ese texto
- echo "texto" > archivo	  Guarda texto en un archivo y reemplaza lo anterior
- echo "texto" >> archivo	  Agrega texto al final del archivo sin borrar
- &&	  Ejecuta el segundo comando cuando termina el primero
- &	  Ejecuta un comando en segundo plano
- Ctrl+C	  Cancela un comando que se quedó esperando
- Errores que cometí (y qué aprendí)
- find -folder ... dio error:   la opción correcta es -name.
- grep "texto" sin archivo se quedó esperando: grep necesita el archivo donde buscar.
- grep no encontró el archivo: yo estaba en otra carpeta; hay que entrar con cd o usar la ruta completa.
- cat carpeta da error porque cat lee archivos, no carpetas.
-Qué me costó
Recordar los comandos sin mirar la pista.
Distinguir > (reemplaza) de >> (agrega).
- Siguiente paso

Practicar sin guía con OverTheWire Bandit (niveles 0 a 10) para fijar estos comandos.
