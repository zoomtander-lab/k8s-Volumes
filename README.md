# ![Laboratirio](https://raw.githubusercontent.com/zoomtander-lab/k8s-Volumes/master/assets/lab.png) Laboratorio de Volumenes en K8s

Laboratorio para realizar pruebas de concepto sobre los volumenes en Kubernetes. En este proyecto se estudiará la mejor alternativa para un Storage en K8s según su rendimiento, escalabilidad y mantenibilidad.

Para ello se evaluan los siguientes protocolos:

* NFS
* GlusterFS
* Ceph
* BeeGFS

## Contexto

Estas pruebas tienen bastantes variables y combinaciones, puesto que no sólo existen distintos proveedores de servicios en la nube, sino que distintos medios para almancenar, distintos tipos de acceso, etc.

Para contextualizar, presentamos las siguientes variables:

### Cloud Providers

* Azure
* AWS
* DO
* GCP

### ReclaimPolicy

* Retain
* Delete
* Recycle

### BoundType

Forma en la que un PVC seleccionará su PV.

* Ninguna: No elige uno, deja que sea asignado de forma arbitraria
* Selector: Utiliza un label para seleccionar un conjunto de PVs
* Nombre: Utiliza un PV en particular

### AccessMode

* ReadWriteOnce
* ReadWriteMany

## Estructura del Proyecto

* GCP
    + ReadWriteOnce
        + Retain
            + Caso1...CasoN
                - assets/
                - README.md
        + Delete
             + Caso1...CasoN
                - assets/
                - README.md
        + Recycle
             + Caso1...CasoN
                - assets/
                - README.md
* Azure
    + ReadWriteOnce
        + Retain
            + Caso1...CasoN
                - assets/
                - README.md
        + Delete
             + Caso1...CasoN
                - assets/
                - README.md
        + Recycle
             + Caso1...CasoN
                - assets/
                - README.md
* DO
    + ReadWriteOnce
        + Retain
            + Caso1...CasoN
                - assets/
                - README.md
        + Delete
             + Caso1...CasoN
                - assets/
                - README.md
        + Recycle
             + Caso1...CasoN
                - assets/
                - README.md
* AWS
    + ReadWriteOnce
        + Retain
            + Caso1...CasoN
                - assets/
                - README.md
        + Delete
             + Caso1...CasoN
                - assets/
                - README.md
        + Recycle
             + Caso1...CasoN
                - assets/
                - README.md

---

## Guía de Usuario

En cada subdirectorio encontrarás un archivo **README.md** con una guía de como ejecutar los pasos necesarios para realizar la prueba, además del contexto actual y prerequisitos.

## Guía de Contribución

Si quieres aportar al proyecto sólo tienes que seguir la guía de contribución en el archivo [CONTRIBUTING.md](https://github.com/zoomtander-lab/k8s-Volumes/blob/master/CONTRIBUTING.md)

## Código de Conducta

El código de conducta establece las normas sociales, reglas y responsabilidades que los individuos y organizaciones deben seguir al interactuar de alguna manera con la herramienta digital o su comunidad. Es una buena práctica para crear un ambiente de respeto e inclusión en las contribuciones al proyecto.

Si quieres aportar al proyecto, te invitamos a revisar el archivo [CODE_OF_CONDUCT.md](https://github.com/zoomtander-lab/k8s-Volumes/blob/master/CODE_OF_CONDUCT.md)

## Agradecimientos y menciones

El ícono de laboratorio simbolico de nuestra organización es creación de [Freepik](https://www.flaticon.es/autores/freepik) ([www.flaticon.es](https://www.flaticon.es/))

## Autores

* Williams Alejandro Gomez Ayala ![Venezuela](https://raw.githubusercontent.com/zoomtander-lab/k8s-Volumes/master/assets/ve.png)
* Marcos Abraham Hernandez Bravo ![Chile](https://raw.githubusercontent.com/zoomtander-lab/k8s-Volumes/master/assets/cl.png)

## Licencia

MIT License, Copyright (c) 2020 Zoomtander-Lab
