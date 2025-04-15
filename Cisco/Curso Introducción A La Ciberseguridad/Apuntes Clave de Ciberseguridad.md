# APUNTES TÉCNICOS DE CIBERSEGURIDAD

CONSIGNA: Responder rápidamente y minimizar el impacto.

# TEMARIO
1. [LA CIBERSEGURIDAD](#la-ciberseguridad)
1. [PRINCIPIOS FUNDAMENTALES DE LA PROTECCION DE LA INFORMACION](#principios-fundamentales-de-la-proteccion-de-la-información)
1. [MEDIDAS PARA LA PROTECCION DE LOS DATOS](#medidas-para-la-protección-de-los-datos)
1. [CONSECUENCIAS DE UNA VIOLACION DE SEGURIDAD](#consecuencias-de-una-violación-de-seguridad)
1. [ALGUNAS PRÁTICAS MEJORADAS DE SEGURIDAD PARA EVITAR LA VIOLACIÓN DE DATOS](#algunas-práticas-mejoradas-de-seguridad-para-evitar-la-violación-de-datos)
    * [Algoritmos de salado](#algoritmos-de-salado) 
1. [FAQ](#faq)

    

# PARTE INTRODUCTORIA

## LA CIBERSEGURIDAD

Se desarrolla en tres ámbitos procurando proteger:

### Individuo

Datos personales, protección de su identidad y dispositivos informáticos.

### Institución

Datos de la compañía, información de los clientes, reputación.

### Gobierno

Juega un papel fundamental en la estabilidad, la economia, la seguridad y el bienestar de los ciudadanos. 

## PRINCIPIOS FUNDAMENTALES DE LA PROTECCION DE LA INFORMACIÓN

### Confidencialidad

Métodos: Cifrado de Datos, Autenticación, Control de Acceso.

### Integridad

Función Hash (ejerce un control en el sistema o la información) o Suma (ver que la data no este alterada) de Comprobación para garantizar la integridad de la información.

### Disponibilidad
Acceso autorizado al sistema donde y cuando sea necesario.
Puntos clave: mantenimiento de hardware, reparaciión de software, actualización de sistemas operativos y software y creación de copias de seguridad.

[👆](#temario)


## MEDIDAS PARA LA PROTECCIÓN DE LOS DATOS

### Concientización
Capacitación y educación acerca de amenazas de seguridad y acciones que se pueden llevar a cabo.

### Tecnología
Firewall (Software o Hardware) para monitorear la red y detectar incidentes maliciosos.

### Política y Procedimiento
se refieren a los controles administrativos que proporcionan una base para la forma en que una organización implementa el aseguramiento de la información, como los planes de respuesta a incidentes y las pautas de mejores prácticas.

[👆](#temario)

## CONSECUENCIAS DE UNA VIOLACIÓN DE SEGURIDAD

### Daño a la reputación
Perdida de credibilidad, empleados que se van. 

### Vandalismo
Modificación de datos con número de teléfono y direcciones en una página web.

### Robo
Violación de datos, robo de información, publicación de información, explotación de información para robar dinero e identidad

### Perdida de ingresos
Eliminación de un sitio web donde se realizan transacciones.

### Propiedad intelectual dañada
Impacta la competitividad por el acceso a documentos confidenciales, secretos comerciales y propiedad intelectual.

[👆](#temario)

## ALGUNAS PRÁTICAS MEJORADAS DE SEGURIDAD PARA EVITAR LA VIOLACIÓN DE DATOS
+ Almacenar las contraseñas de los clientes mediante una combinación de algoritmos de salado y hash robustos.
+ Separar los recursos basados en la nube de la Internet pública en un segmento de red privada aislada.
+ Conceder a los empleados acceso a los datos personales y a los sistemas internos solo a través de una conexión VPN segura.

### Algoritmos de salado
Los algoritmos de salado son un sistema de cifrado que agrega datos aleatorios a las contraseñas antes de aplicar un algoritmo hash. Esto se hace para proteger las contraseñas de ataques de diccionario y de tablas arcoíris. 

Cómo funciona 

    Se genera aleatoriamente una sal para cada contraseña.
    Se concatena la sal con la contraseña.
    Se procesa la cadena con una función hash criptográfica.
    El resultado se almacena en una base de datos junto con la sal. 

Ventajas del salado

    Cada hash de contraseña es único, incluso si las contraseñas son idénticas. 

Protege las contraseñas comunes o a quienes usan la misma contraseña en varios sitios. 
Dificulta que los atacantes intenten comprometer las cuentas de usuario. 

Recomendaciones 

    La sal de contraseña debe ser aleatoria, larga, compleja e imposible de predecir.
    Se debe generar una nueva sal cada vez que un usuario cambie su contraseña o cree una nueva cuenta.

PARA TRABAJAR

    Registrar hallazgos (brechas de seguridad)

[👆](#temario)

## GLOSARIO

+ Cluster: grupo de servidores vinculados que proporcionan almacenamiento de datos, bases de datos, redes y software a través de Internet.

+ DDoS: ataques de denegación de servicios distribuidos. Se produce cuando varios dispositivos infectados con malware inundan recursos de un sistema objetivo.

+ Exploit: software malicioso que aprovecha errores de un sistema para robar información, instalar malware, o tomar control de un ordenador.


[👆](#temario)




