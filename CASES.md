# Pruebas de Volumenes en Kubernetes (K8s)

Casos de Prueba

1.- Escenario Feliz (1D + 1PV + 1 PVC + 2PD)
   Caso 1: Crear archivo y recrear pod.
         * ka PersistentVolume.yml
         * ka PersistentVolumeClaim.yml
         * ka Deployment.yml
         * ke dm-timer bash
         * echo hola > /timer/a.txt
         * exit
         * kd Deployment.yml
         * ka Deployment.yml
         * ke dm-timer bash
         * cat /timer/a.txt
      
      Resultado: No se borra nada.
   
   Caso 2: Borrar pvc
         * ka PersistentVolume.yml
         * ka PersistentVolumeClaim.yml

         * kd PersistentVolumeClaim.yml
         * ka PersistentVolumeClaim.yml
         
      Resultado: Crea un nuevo Vola
   
   
   
   1 pv + 1 pvc + 1 pod:
    - Retain:

    - Recycle:

    - Delete:
        
