---
templateKey: blog-post
title: Licencias de Cloud Berry VM
date: 2020-01-08T18:30:50.751Z
description: >-
  Recientemente compré unas licencias de CloudBerry VM, con lo cual he aprendido
  de mejor manera como funciona su modelo de licencias. Les comparto los
  detalles que considero más importantes. 
featuredpost: true
featuredimage: /img/blog-index.jpg
tags:
  - aws
  - cloudberry
  - vm
  - dr
---
## Tipos de licencia

* **Licencia Perpetua (clásica)**. Los precios son públicos. Actualizaciones únicamente por año. No existe un panel de administración para gestionar todas las instalaciones. 
* **Licencia Anual.** Los precios son privados (Se debe de hacer login para tener acceso a los precios). Las actualizaciones siempre están disponibles media vez la licencia tenga validez. Administración centralizada (Creación de usuarios, Quotas, Destinos, Rebranding). Existe descuentos por volumen. Generalmente un año cuesta 50% menos que la licencia perpetua. 

## CloudBerry VM

CloudBerry VM sirve para hacer backup de servidores virtuales, que utilizan VMWare o HyperV como Hypervisor. Es necesario tener espacio para Snapshots en el Data Center Local ya que CloudBerry lo que sube a la nube es una copia del Snaphost de la VM. Las VMs pueden restaurarse en AWS, Azure o Google Cloud. 

**El licenciamiento** es por Socket y cuesta $300 en licencia perpetua y $150 con licencia anual. Esta licencia "inicial" trae ya incluidos dos Sockets. Cada Socket adicional tiene un precio de $150 en licencia perpetua y $79 con licencia Anual.

**Ejemplo**. Se tiene un cluster de VMWare 4 nodos y cada nodo tiene 2 sockets, con lo cual se tiene un cluster de 8 sockets. Entonces se debería de comprar la licencia inicial (2 sockets) y 6 licencias de sockets adicionales. 

Como recomendación se deberían de adquirir licencias anuales ya que nos dan más flexibilidad en la administración, podemos hacer rebranding (poner el logo de nuestra empresa en el software) y se apaga mucho más a un modelo de cobro anual que es el que generalmente utilizan las empresas.
