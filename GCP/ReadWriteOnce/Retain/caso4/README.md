Caso 4

* ka PersistentVolume.yml
* ka PersistentVolumeClaim.yml

* kd PersistentVolumeClaim.yml
* ka PersistentVolumeClaim.yml

* kd PersistentVolume.yml
* ka PersistentVolume.yml

Resultado: Se resuelve el pvc y conecta con el pv. Solo se puede desbloquear un pv recreandolo.
Detalle: Se indica a pvc el nombre del "pv-timer".
