# TEMARIO
1. [GIT](#git)
    * [Configuración global](#configuración-global) 
    * [Subir un repositorio local a GitHub](#subir-un-repositorio-local-a-github)
    * [Mostrar los mensajes de los últimos commits](#mostrar-los-mensajes-de-los-últimos-commits)
1. [VIRTUALBOX](#virtualbox)
    * [Instalar Guest Additions desde repositorios](#instalar-guest-additions-desde-repositorios)
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

## Mostrar los mensajes de los últimos commits

git log

ó 

git log -n 5 mostrará los últimos 5 commits

ó 

git log -1 para mostrar el mensaje del último commit

[👆](#temario)

# VIRTUALBOX

## Instalar Guest Additions desde repositorios

sudo apt-get install virtualbox-guest-additions-iso

La archivo de imagen .iso de la guest additions CD se instala en la ruta /usr/share/virtualbox/VBoxGuestAdditions.iso. 

[👆](#temario)

## GLOSARIO

**[A](#a)** - **[B](#b)** - **[C](#c)** - **[D](#d)** - **[E](#e)** - **[F](#f)** - **[G](#g)** - **[H](#h)** - **[I](#i)** - **[J](#j)** - **[K](#k)** - **[L](#l)** - **[M](#m)** - **[N](#n)** - **[Ñ](#ñ)** - **[O](#o)** - **[P](#p)** - **[Q](#q)** - **[R](#r)** - **[S](#s)** - **[T](#t)** - **[U](#u)** - **[V](#v)** - **[W](#w)** - **[X](#x)** - **[Y](#y)** - **[Z](#z)**


[👆](#temario)

