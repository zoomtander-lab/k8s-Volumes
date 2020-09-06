Caso 2

* ka PersistentVolume.yml
* ka PersistentVolumeClaim.yml

* kd PersistentVolumeClaim.yml
* ka PersistentVolumeClaim.yml

Resultado: No usa "pv-timer" y no puede crear el pvc ni un volumen dinamico.

Error:
    Failed to provision volume with StorageClass "standard": claim.Spec.Selector is not supported for dynamic provisioning on GCE.

Detalle: Se agrega grupo y selector.
