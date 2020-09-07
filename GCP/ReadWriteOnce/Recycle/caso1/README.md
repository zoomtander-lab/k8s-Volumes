# GCP-RWO-RC-C1: Recrear un PVC

Probaremos el comportamiento de un PV asociado a un PVC.

## Diagrama

![Diagrama](https://raw.githubusercontent.com/zoomtander-lab/k8s-Volumes/master/GCP/ReadWriteOnce/Recycle/caso1/assets/diagrama.png)

**Requisitos**:

* Crear disco en [Compute Engine](https://console.cloud.google.com/compute/disks) llamado "**dsk-timer**"

**Setup**:

```bash
    kubectl apply -f PersistentVolume.yml
    kubectl apply -f PersistentVolumeClaim.yml
```

Creamos el PersistentVolume (pv) y le asociamos un PersistentVolumeClaim (pvc).

![alt](https://link)

**Prueba**:

```bash
    kubectl delete -f PersistentVolumeClaim.yml
    kubectl apply -f PersistentVolumeClaim.yml
```

Resultado: Crea un nuevo volumen dinamico. No usa "pv-timer".


## Autores

* Williams Alejandro Gomez Ayala ![Venezuela](https://raw.githubusercontent.com/zoomtander-lab/k8s-Volumes/master/assets/ve.png)(Venezuela)
* Marcos Abraham Hernandez Bravo ![Chile](https://raw.githubusercontent.com/zoomtander-lab/k8s-Volumes/master/assets/cl.png)(Chile)

## Licencia

MIT License, Copyright (c) 2020 Zoomtander-Lab
