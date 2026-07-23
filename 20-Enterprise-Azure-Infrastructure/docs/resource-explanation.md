# Explicación Técnica de la Infraestructura



---



# Microsoft Entra ID



## Función



Microsoft Entra ID proporciona autenticación e identidad para administrar los recursos de Azure de forma segura.



## Justificación



Se utiliza para controlar el acceso administrativo a toda la infraestructura mediante identidades centralizadas.



---



# Azure Subscription



## Función



La suscripción representa el límite administrativo donde se implementan todos los recursos de Azure.



## Justificación



Permite organizar el consumo, costos, permisos y administración general de la infraestructura.



---



# Resource Group



## Recurso



RG-LAB-AZ104



## Función



Agrupa todos los recursos relacionados con el proyecto.



## Justificación



Facilita la administración, automatización, monitoreo y eliminación conjunta de los recursos.



---



# Virtual Network



## Recurso



VNET-LAB01



## Función



Proporciona la red privada donde se implementan los recursos principales.



## Justificación



Permite la comunicación segura entre máquinas virtuales y servicios internos.



---



# Virtual Machine



## Recurso



VM-WIN01



## Función



Servidor principal utilizado para ejecutar las cargas de trabajo del laboratorio.



## Justificación



Representa el recurso principal donde se implementan aplicaciones y servicios.



---



# Virtual Machine Scale Set



## Recurso



VMSS-LAB01



## Función



Permite aumentar o disminuir automáticamente la cantidad de máquinas virtuales.



## Justificación



Implementa escalabilidad horizontal según la demanda de la aplicación.



---



# Azure Load Balancer



## Recurso



LB-LAB01



## Función



Distribuye el tráfico entre múltiples instancias.



## Justificación



Mejora la disponibilidad y evita puntos únicos de falla.



---



# Azure VPN Gateway



## Recurso



VPNGW-LAB01



## Función



Permite la conectividad segura entre Azure y redes externas.



## Justificación



Hace posible implementar escenarios híbridos.



---



# Azure Key Vault



## Recurso



kv-joseduver-104



## Función



Almacena secretos, certificados y claves de cifrado.



## Justificación



Evita almacenar credenciales directamente dentro de aplicaciones o máquinas virtuales.



---



# Azure Storage Account



## Recurso



stjoseduver01



## Función



Servicio de almacenamiento para archivos y datos.



## Justificación



Permite almacenar información altamente disponible y escalable.



---



# Recovery Services Vault



## Recurso



RSV-LAB-AZ104



## Función



Administra copias de seguridad y recuperación ante desastres.



## Justificación



Protege la continuidad operativa de la infraestructura.



---



# Azure Monitor



## Función



Recopila métricas, registros y eventos de toda la infraestructura.



## Justificación



Permite detectar problemas de rendimiento y generar alertas.



---



# Microsoft Defender for Cloud



## Función



Supervisa continuamente la postura de seguridad del entorno.



## Justificación



Identifica vulnerabilidades y genera recomendaciones para mejorar la seguridad.

