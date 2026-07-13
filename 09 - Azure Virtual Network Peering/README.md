# 🌐 Azure Virtual Network Peering



## 📌 Objetivo



Implementar Azure Virtual Network Peering para permitir la comunicación privada entre dos redes virtuales dentro de la misma suscripción y región de Azure.



---



# 🏗️ Arquitectura



```

              Azure Subscription



             RG-LAB-AZ104

                      │

     ┌────────────────┴────────────────┐

      │                                 │

 VNET-LAB01                       VNET-LAB02

 10.0.0.0/16                      10.1.0.0/16

     │                                 │

 VM-WIN01                         (Sin VM)

 VM-WIN02

   │

   └──────────── Peering ────────────┘

```



---



# 🎯 Objetivos del laboratorio



- Crear una segunda Virtual Network.

- Configurar Virtual Network Peering.

- Permitir la comunicación entre ambas redes virtuales.

- Comprender el funcionamiento del emparejamiento de redes en Azure.

- Validar el estado del peering.



---



# 🛠️ Recursos utilizados



| Recurso | Nombre |

|----------|---------|

| Resource Group | RG-LAB-AZ104 |

| Virtual Network | VNET-LAB01 |

| Virtual Network | VNET-LAB02 |

| Virtual Network Peering | VNET01-to-VNET02 |

| Virtual Network Peering | VNET02-to-VNET01 |



---



# 📷 Evidencias



## 1. Creación de la segunda Virtual Network



![01](images/01-create-vnet-lab02.png)



---



## 3. Estado Connected del Peering



![03](images/03-peering-connected.png)



---



# 🔍 Verificación



Se comprobó que:



- Ambas Virtual Networks pertenecen a la misma región (\*\*East US 2\*\*).

- Los espacios de direcciones IP no se superponen.

- El Virtual Network Peering quedó en estado \*\*Connected\*\*.

- Se habilitó el acceso entre ambas redes virtuales.



---



# ⚠️ Limitación encontrada



La suscripción utilizada para el laboratorio tiene una cuota limitada de vCPU para la familia \*\*Standard\_D2s\_v3\*\*.



Actualmente las máquinas virtuales:



- VM-WIN01

- VM-WIN02



consumen la totalidad de la cuota disponible.



Por este motivo no fue posible crear una tercera máquina virtual dentro de \*\*VNET-LAB02\*\* para realizar pruebas de conectividad entre ambas redes.



La configuración del Virtual Network Peering quedó implementada correctamente y lista para ser utilizada cuando exista capacidad disponible para implementar recursos adicionales.



---



# 📚 Conceptos aprendidos



- Azure Virtual Networks

- Address Spaces

- Subnets

- Virtual Network Peering

- Comunicación privada entre VNets

- Configuración de acceso entre redes

- Limitaciones de cuotas (vCPU Quotas)



---



# 💡 Conclusiones



Azure Virtual Network Peering permite conectar dos redes virtuales de manera privada utilizando la infraestructura de Microsoft, sin necesidad de utilizar Internet pública.



Durante este laboratorio se implementó correctamente el emparejamiento entre dos redes virtuales y se verificó su estado de funcionamiento. La validación mediante máquinas virtuales quedó pendiente debido a una limitación de cuota de la suscripción utilizada para el laboratorio, situación común en entornos de prueba y laboratorio.



---



