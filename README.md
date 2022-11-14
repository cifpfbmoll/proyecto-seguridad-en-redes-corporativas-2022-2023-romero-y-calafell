# proyecto-seguridad-en-redes-corporativas-2022-2023-romero-y-calafell
proyecto-seguridad-en-redes-corporativas-2022-2023-romero-y-calafell created by GitHub Classroom

Sprint 1 - Hardening de Ubuntu

US2 (fecha tope 21 de octubre): CA 3.  El servidor de la empresa tendrá como S.O. Ubuntu, que incorporará las medidas de seguridad correspondientes.
Instala Ubuntu y aplica las configuraciones que se comentan en el seminario de Incibe. Aunque en el seminario se describen muchas más configuraciones, y es interesante que visualices completamente la guía, solo debes aplicar las configuraciones que se describen a continuación.
Asegura las configuraciones globales.
Configuración del arranque GRUB.
Establecer una contraseña de arranque.
Establecer permisos fichero de configuración de arranque
Obligar al uso de contraseña en el modo “single user”

Configuración de usuarios y grupos. Crea un usuario administrador con tu nombre, y añade este al grupo sudoers. Además, aplica  una política de contraseñas adecuada. 
Complejidad
Reutilización de contraseñas.
Almacenamiento de contraseñas. Comprueba como un hash puede ser roto si el cifrado no es el adecuado. Sigue este tutorial.
Ahora ya has evidenciado la importancia de realizar almacenamiento seguro de contraseñas como por ejemplo sha512. Una vez establecido vuelve a proceder el ataque.
Configuración del entorno (Caducidad y cambio de contraseña, Timeout de inactividad, Bloqueo de cuenta tras varios intentos, etc)

Actualizaciones de software.


Sprint 2 - Hardening de Windows

US3: (fecha tope 27 octubre) CA 3.  Los equipos de los empleados son ordenadores portátiles, ya que necesitan en ocasiones teletrabajar.
Instala un S.O Windows 11 o 10. Para simular en mejores condiciones la red local de los empleados del entono empresarial, este equipo Windows 10 tendrá un usuario local (tu nombre y apellidos, sin active directory) 
Este equipo será utilizado por un empleado que tendrá mínimos privilegios (no podrá instalar nada), por tanto, debe existir otro usuario administrador. Crea los dos usuarios con los privilegios adecuados, y comprueba su configuración.
Desinstalar programas que no estemos usando. Es peligroso que haya software que como administradores no tengamos controlada sus versiones. Como en el punto anterior hemos limitado la instalación a nuestro empleado en cuestión, podríamos decir que no debe haber programas no autorizados.
Utilizar Seguridad de Windows. Comprueba que efectivamente tienes habilitado Windows Defender. 
Comprueba que tienes habilitado la protección contra ransomware. 
Acceso controlado a carpetas: es sumamente importante mantenerlo activo. Ya que esto permitirá que potenciales programas maliciosos no puedan tener control de tus archivos y carpetas. Además, tendrás opción de visualizar el historial de los bloqueos, agregar o quitar carpetas protegidas y gestionar las aplicaciones que tienen acceso controlado a tus archivos o carpetas. Comprueba que tienes protegida la carpeta de Documentos del perfil del usuario, ya que esta es la carpeta que utilizará el usuario para el trabajo diario.
Recuperación de datos por ransomware: si utilizas OneDrive, podrás configurar y gestionar la sincronización de tus archivos y carpetas (para nuestro caso, no es necesario, simplemente es que informativo este paso para que sepáis que existe). Esto será de gran utilidad, sobre todo, si es que llegas a ser víctima de este tipo de ataque, ya que todos los archivos estarán en tu espacio en la nube. Así también, ten presente que todos los cambios que hagas en los archivos sincronizados, los mismos se verán reflejados en la sincronización con OneDrive en sí. 

Comprueba que si hubiera un intento de intrusión en uno de los portátiles si podrían resetear la contraseña del administrador y acceder a la cuenta.




Ya has visto el peligro que supone el arranque de herramientas live. Aplica las medidas necesarias para contrarrestar este riesgo:
Adecuada política de contraseñas: caducidad contraseñas, longitud, simbolos, etc.
Cifrado de disco. 
Comenta como evitas el arranque de herramientas live.
