# Proyecto 01 - Implementación de una infraestructura básica en Microsoft Azure

## Objetivo

Implementar una infraestructura básica en Azure utilizando redes virtuales, grupos de seguridad y una máquina virtual Windows.

---

## Recursos implementados

- Resource Group: RG-LAB-AZ104
- Virtual Network: VNET-LAB01
- Subnet: SUBNET-SERVERS
- Network Security Group: NSG-LAB01
- Windows Server 2022 Virtual Machine
- Public IP
- Network Interface
- Managed Disk

---

## Arquitectura

```
RG-LAB-AZ104
│
├── VNET-LAB01
│     └── SUBNET-SERVERS
│
├── NSG-LAB01
│
├── VM-WIN01
│
├── Public IP
│
├── Network Interface
│
└── Managed Disk
```

---

## Evidencias

### Resource Group

![Resource Group](images/resource-group-created.png)

### Virtual Network

![Virtual Network](images/vnet-created.png)

### Network Security Group

![NSG](images/nsg-created.png)

### Máquina Virtual

![VM](images/vm-created.png)

### Conexión por RDP

![RDP](images/rdp-connected.png)

---

## Problemas encontrados

Durante la implementación se presentaron los siguientes inconvenientes:

- Registro del proveedor **Microsoft.Compute**.
- Restricción de Availability Zone.
- Restricción de tamaños de VM disponibles.
- Configuración del acceso RDP mediante Network Security Group.

---

## Conocimientos aplicados

- Azure Resource Groups
- Azure Virtual Networks
- Azure Subnets
- Network Security Groups
- Azure Virtual Machines
- Public IP
- Remote Desktop (RDP)
- Administración básica de infraestructura Azure

---

## Resultado

La infraestructura fue desplegada correctamente y se logró el acceso remoto a la máquina virtual mediante RDP.