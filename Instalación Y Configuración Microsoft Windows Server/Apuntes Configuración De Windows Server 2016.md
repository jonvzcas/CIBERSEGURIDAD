## EDICIONES

**Essential**\
Pequeñas empresas\
25 users 50 PC\
Puede venir en OEM - Hardware\
No tiene todos los roles como Hyper-V
Incluye las CAls de acceso remoto

**Standar | Datacenter**\
Mismos roles y caracteristicas\
Diferencia: En la versión Standar se pueden ejecutar 2MV gratuitamente. En la Datacenter ilimitadamente.\
Costo: Standar -> 800 USD, Datacenter -> 2500 USD
Adicionalmente comprar las CALs RDS para la conexión remota de las maquinas

**Azure**\
Solo se ejecutan en el servicio de Azure VM
o de forma local con Azure Stack HCI
Hotpatching  

## Web para descargar actualizaciones manualmente de Microsoft

Desde el catalogo de Microsoft Update, paquetes de actualización acumulativa.

www.catalog.update.microsoft.com


## COMANDOS

* Mostrar el rastreados de eventos (_para apagado_): Alt + F4
* Mostrar la versión instalada de Windows Server: DISM /online /Get-CurrentEdition
* Activar la versión de Windows: DISM /online /Set-Edition:ServerStandard /ProductKey:VDYBN-27WPP-V4HQT-9VMD4-VMK7H /AcceptEula
* Cambiar la clave del producto: slmgr ipk XXXXX-XXXXX-XXXXX-XXXXX-XXXXX

  luego de eso, para activar la clave ejecutamos: slmgr -auto   
