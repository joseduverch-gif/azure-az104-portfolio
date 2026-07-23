# Inventario de la Infraestructura



## Resource Group



| Recurso | Nombre |
|----------|--------|
| Resource Group | RG-LAB-AZ104 |



---



# Recursos implementados



| Recurso | Nombre | Propósito |
|----------|--------|-----------|
| Microsoft Entra ID | Directorio predeterminado | Administración de identidades |
| Azure Subscription | Azure subscription 1 | Administración de recursos |
| Virtual Network | VNET-LAB01 | Red principal |
| Virtual Network | VNET-LAB02 | Red secundaria para conectividad |
| Virtual Machine | VM-WIN01 | Servidor principal |
| Virtual Machine Scale Set | VMSS-LAB01 | Escalabilidad automática |
| Load Balancer | LB-LAB01 | Distribución del tráfico |
| VPN Gateway | VPNGW-LAB01 | Conectividad híbrida |
| Public IP | PIP-LB01 | Acceso al Load Balancer |
| Public IP | PIP-VPNGW01 | Acceso al VPN Gateway |
| Public IP | VM-WIN01-ip | Acceso remoto a la VM |
| Network Security Group | NSG-LAB01 | Seguridad de red |
| Route Table | RT-LAB01 | Enrutamiento personalizado |
| Storage Account | stjoseduver01 | Almacenamiento |
| Key Vault | kv-joseduver-104 | Administración de secretos |
| Recovery Services Vault | RSV-LAB-AZ104 | Copias de seguridad |
| Azure Monitor | High-CPU-VM-WIN01 | Supervisión |
| Action Group | AG-CPU-Alert | Notificaciones |
| Snapshot | Snapshot-VM-WIN01 | Recuperación del disco |
| Managed Disk | VM-WIN01\_OsDisk | Disco administrado |
| Network Interface | vm-win01341 | Interfaz de red |
| Basic NSG | basicNsgVNET-LAB01-nic01 | Seguridad de NIC |
