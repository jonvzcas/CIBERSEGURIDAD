# TEMARIO
1. [GIT](#git)
    * [Configuración global](#configuración-global) 
1. [ENCRIPTADO Y SEGURIDAD](#encriptado-y-seguridad)
    * [Función Hash](#función-hash)


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

# ENCRIPTADO Y SEGURIDAD

## Función Hash
Ver el siguiente [articulo ](https://latam.kaspersky.com/blog/que-es-un-hash-y-como-funciona/2806/?srsltid=AfmBOooiZ2uPfrDTyFWtrTLJ8MFUHIPD-XxlfoZh-WD92jWej_oQS8IM) en la web de Kaspersky

[👆](#temario)