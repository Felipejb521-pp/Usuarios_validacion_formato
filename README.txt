Este proyecto presenta un sistema de almacenamiento de datos de usuarios en formato XML, validado mediante un esquema XSD personalizado. El objetivo es asegurar que la información crítica (emails, teléfonos, códigos postales y contraseñas) cumpla con estándares de formato específicos.

Contenido del Repositorio
	usuarios.xml: Archivo de datos con ejemplos de usuarios.usuarios.xsd: 
	Esquema de validación con reglas de tipos simples y complejos.
	video_demo.mp4: Demostración visual del funcionamiento y validación. 

Reglas de Validación (XSD)
El archivo usuarios.xsd aplica las siguientes restricciones mediante Expresiones Regulares (Regex):
	
	Email
		Formato estándar (usuario@dominio.tld) con longitud controlada.
	Teléfono 
		Debe incluir el prefijo de España +34 seguido de 9 dígitos.
	Código Postal 
		Limitado estrictamente a España (01-52) con 5 dígitos exactos.
	Nombre de Usuario
		Mínimo 6 caracteres en minúscula, empezando por letra o número y permitiendo . o _.
	Contraseña
		Mínimo 8 caracteres, alfanumérica con caracteres especiales permitidos.
