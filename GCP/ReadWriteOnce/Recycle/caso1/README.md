# GCP-RWO-RC-C1: Recrear un PVC

Probaremos el comportamiento de un PV asociado a un PVC.

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


>Ver: [Abreviaturas, siglas y acrónimos](https://github.com/zoomtander-lab/k8s-Volumes/blob/master/ABBREVIATIONS.md)
