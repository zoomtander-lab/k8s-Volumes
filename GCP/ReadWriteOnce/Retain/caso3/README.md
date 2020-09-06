Caso 3

* ka PersistentVolume.yml
* ka PersistentVolumeClaim.yml

* kd PersistentVolumeClaim.yml
* ka PersistentVolumeClaim.yml

Resultado: Asigna el volume "pv-timer", pero no puede conectarse a el por que queda bloqueado. Queda el pvc en estado "Pending" eternamente. El pv queda bloquedo.

Detalle: Se indica a pvc el nombre del "pv-timer".
