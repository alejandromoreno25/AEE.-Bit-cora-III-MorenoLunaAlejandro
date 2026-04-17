## **FASE NÚMERO 1:**

Cuando nosotros instalamos un servicio en Linux, necesitamos saber si al configurarlo todo está saliendo según lo previsto. Todo esto, podemos conseguirlo a través del Syslog.

Syslog es un protocolo es decir, un conjunto de normas o pautas en la que los dispositivos usan un mensaje para comunicarse con un servidor. Esto, fué diseñado para facilitar la gestión de los dispositivos de red. En resumen, es lo que hace que los dispositivos se puedan conectar al servidor en linux.

Debido a la gran cantidad de eventos que tiene que gestionar Syslog, nos proporciona dos campos llamados Facility and Severity que los usa Syslog para mostrar la importancia de un mensaje. En concreto,el facility nos ayuda a clasificar de donde viene ese mensaje y dependiendo de donde venga puede tener una gravedad u otra. como por ejemplo que venga del Kernel.**\[1\] \[2\]** 

Estos valores, van entre 0 y 7 dependiendo del grado de emergencia del aviso:   
como por ejemplo 1:EMERGENCIA u 8:DEPURACIÓN.

**¿Por qué es una negligencia grave que el archivo */var/log/auth.log* tenga permisos de lectura para usuarios no privilegiados?**

El fichero /var/log/Auth.log. es un fichero que almacena toda la autorización del equipo. Como por ejemplo, cuando un usuario inicia sesión en el sistema. Esto puede llegar a ser muy grave porque se pueden llegar a filtrar todos los datos. **\[1\]\[3\]\[4\]**

**¿Qué información específica (como PIDs, nombres de usuario o direcciones IP) diferencia un intento fallido de conexión remota *SSH* de un simple fallo de contraseña de un usuario local frente a la pantalla?**

La diferencia entre diferenciar un intento fallido de la conexión remota o un simple fallo de contraseña, es que cuando el fallo viene del SSH es decir el secure shell que es lo que nos ayuda a administrar los servidores el sistema apunta tu IP porque el fallo viene de afuera. En cambio, si es local el sistema no lo realiza y manda el fallo como Login.**\[4\]**

## **FASE NÚMERO 2:**

**Busca en Dialnet o Semantic Scholar artículos sobre *Log Management* (Gestión centralizada de registros). A nivel empresarial y legal (piensa en el RGPD en España), ¿qué ventajas vitales ofrece enviar y custodiar los logs en un servidor externo seguro en lugar de mantenerlos dispersos e indefensos en la propia máquina que podría ser vulnerada?**

El Log Management es el proceso de guardar y analizar todos los mensajes que generan nuestros equipos para saber que pasa en todo momento.

Las ventajas vitales de enviar los logs en servidores externos es que por ejemplo si un hacker entra en nuestro equipo, evitamos que nos borre sus huellas de su ataque ya que el log management almacena todos esos datos en un lugar seguro además, de vigilar tus máquinas.

## **BIBLIOGRAFÍA:**

\[1\] Syslog conceptos y configuraciones.[https://juncotic.com/aprendiendo-syslog/](https://juncotic.com/aprendiendo-syslog/) 

\[2\] Que es un Servidor Syslog [https://www.whatsupgold.com/es/blog/que-es-un-servidor-syslog-y-como-funciona](https://www.whatsupgold.com/es/blog/que-es-un-servidor-syslog-y-como-funciona)

\[3\] Introducción a los Servidores Syslog [https://blog.invgate.com/es/que-es-syslog](https://blog.invgate.com/es/que-es-syslog) 

\[4\] Gemini [https://gemini.google.com/app](https://gemini.google.com/app) 