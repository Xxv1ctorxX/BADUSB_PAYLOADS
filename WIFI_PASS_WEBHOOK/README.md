Este payload extrae los 4 primeros perfiles de red WiFi del dispositivo, además de sus contraseñas en claro.
Posteriormente, se almacena esta información en un archivo en la carpeta personal llamado 'pass.txt'.
Luego, se guarda el contenido de 'pass.txt' en una variable y se convierte mediante una serie de comandos, seguidamente se envía al webhook especificado.
Después de enviarlo, se elimina el archivo 'pass.txt' y se limpia el historial de PowerShell. Por último, se cierra la terminal.

Si su dispositivo se ajusta correctamente a los tiempos de DELAY que he establecido, debería tardar aproximadamente 10 segundos en completar todo el proceso.

Este payload está pensado por defecto para dispositivos Windows con el idioma del sistema operativo en español, en caso de que esté en otro idioma, deberá realizar cambios que se indican abajo.

<h1>Instrucciones</h1>

<h4>1. Edita el payload</h4>
<h4>2. Busca en el código la sección "$webhook = "URL_WEBHOOK"</h4>
<h4>3. Reemplaza "URL_WEBHOOK" por la URL de tu webhook, ya sea el de Discord u otro que tengas.</h4>
- Mi recomendación es Discord, donde puedo asegurar su funcionamiento.
<h4>4. Ya lo tienes listo.</h4>
<br>
<br>
<h1>¿Que puedo hacer si el Sistema Operativo está en otro idioma?</h1>
<h4>1. Edita el payload.</h4>
<h4>2. Busca en el código la sección: Select-String (?<=Perfil de todos los usuarios\s+:\s).+ }.</h4>
<h4>3. Edita "Perfil de todos los usuarios", deberás traducirlo al idioma del sistema operativo. (Todos los del payload)</h4>
<h4>4. Busca en el código la sección: Select-String (?<=Contenido de la clave\s+:\s).+ }.</h4>
<h4>5. Edita "Contenido de la clave", deberás traducirlo al idioma del sistema operativo. (Todos los del payload)</h4>
<br>
<br>
<h4>(No me hago responsable del uso ilegal de este payload, recuerda utilizarlo en ambientes controlados y con consentimiento)</h4>

<h6>Este payload está diseñado únicamente con fines legítimos, como la realización de pruebas de seguridad en entornos controlados o la demostración de vulnerabilidades en sistemas propios. Se prohíbe estrictamente el uso indebido o ilegal de este payload. El usuario asume la responsabilidad total de cualquier acción realizada con el payload y debe cumplir con todas las leyes y regulaciones aplicables en su jurisdicción. Cualquier violación de estos términos puede tener consecuencias legales.</h6>
<h6>Por favor, utilice este payload con responsabilidad y en un entorno adecuado, asegurándose de obtener el consentimiento y permisos necesarios antes de su utilización.</h6>
