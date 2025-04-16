# TEMARIO
1. [GIT](#git)
    * [Configuración global](#configuración-global) 
    * [Subir un repositorio local a GitHub](#subir-un-repositorio-local-a-github)
1. [ENCRIPTADO Y SEGURIDAD](#encriptado-y-seguridad)
    * [Función Hash](#función-hash)
1. [ATAQUES CIBERNETICOS](#ataques-ciberneticos)
    * [Ransomware LockBit](#ransomware-lockbit)
1. [GLOSARIO](#glosario)


# GIT

## Configuración global
El usuario A realiza un push a su repositorio, pero al verificar el autor del commit aparece el usuario B 

¿Por que pasa esto?

Eso sucede generalmente porque la configuración de Git (nombre y correo del autor) en la máquina donde se hizo el commit está asociada al usuario B, no al usuario A.

Git identifica a los autores de los commits basándose en dos valores que se configuran a nivel global o por repositorio:

git config user.name "Nombre"

git config user.email "correo@example.com"

Entonces, aunque el usuario A haya hecho el push al repositorio (por ejemplo, usando sus credenciales o SSH key), si los commits fueron creados en una máquina donde Git tiene configurado el nombre y correo de usuario B, los commits aparecerán firmados por usuario B.

¿Cómo solucionarlo?

Verifica la configuración de Git:

git config --global user.name

git config --global user.email

Cámbialo si es necesario:

git config --global user.name "Usuario A"

git config --global user.email "a@example.com"

> [!Note]
>
> Configurarlo en un repositorio especifico 

git config user.name "Usuario A"

git config user.email "a@example.com"

[👆](#temario)

## Subir un repositorio local a GitHub

git branch -M main

git remote add origin https://github.com/xxxxx/xxxxx.git

git push -f -u origin main

[👆](#temario)

# ENCRIPTADO Y SEGURIDAD

## Función Hash
Ver el siguiente [articulo](https://latam.kaspersky.com/blog/que-es-un-hash-y-como-funciona/2806/?srsltid=AfmBOooiZ2uPfrDTyFWtrTLJ8MFUHIPD-XxlfoZh-WD92jWej_oQS8IM) en la web de Kaspersky

[👆](#temario)

# ATAQUES CIBERNETICOS

## Ransomware LockBit

Ver el siguiente [articulo](https://latam.kaspersky.com/resource-center/threats/lockbit-ransomware?srsltid=AfmBOoqg5UKyv5xsX8-zKwV8hq4TOFBTZaYbROcgmL0Ijx0e3umWVWuF)

[👆](#temario)

# GLOSARIO

+ CSIRT: son las siglas en inglés de “Computer Security Incident Response Team”, que se traduce como Equipo de Respuesta a Incidentes de Seguridad Informática. Se trata de un grupo especializado que gestiona las consecuencias de ataques cibernéticos o brechas de seguridad. 

+ Data Leak: una fuga de datos se refiere a información confidencial o sensible que se expone de forma no intencionada o accidental, ya sea externa o internamente, debido a medidas de seguridad insuficientes. [Más detalles.](https://www-paloaltonetworks-co-uk.translate.goog/cyberpedia/data-leak?_x_tr_sl=en&_x_tr_tl=es&_x_tr_hl=es&_x_tr_pto=tc)

+ EDR: detección y respuesta de endpoints, o EDR, es un software que utiliza análisis en tiempo real y automatización impulsada por IA para proteger a los usuarios finales, los dispositivos de puntos finales y los activos de TI de una organización contra las ciberamenazas que eluden el software antivirus y otras herramientas tradicionales de seguridad de puntos finales.

+ SIEM: Security Information and Event Management (Gestión de Eventos e Información de Seguridad), es una solución de ciberseguridad que permite a las organizaciones recopilar, correlacionar, analizar y responder a eventos de seguridad en tiempo real. Sirve para detectar amenazas, investigar incidentes y garantizar el cumplimiento normativo. 

+ SOARD: (orquestación, automatización y respuesta de seguridad) es una solución de software que permite a los equipos de seguridad integrar y coordinar herramientas de seguridad independientes, automatizar tareas repetitivas y agilizar los flujos de trabajo de respuesta a incidentes y amenazas.


[👆](#temario)

