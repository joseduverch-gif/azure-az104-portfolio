# Project 16 - Azure VPN Gateway

## Objective

Deploy an Azure VPN Gateway to provide secure connectivity between Azure virtual networks and on-premises environments using a Virtual Network Gateway.

---

# Architecture

Azure Subscription

↓

Resource Group

↓

VNET-LAB01

├── Subnet

├── GatewaySubnet

↓

VPN Gateway

↓

Public IP

---

# Resources Used

| Resource | Name |
|----------|----------------|
| Virtual Network | VNET-LAB01 |
| Gateway Subnet | GatewaySubnet |
| VPN Gateway | VPNGW-LAB01 |
| Public IP | PIP-VPNGW01 |

---

# Deployment

## Step 1

Created a dedicated Public IP Address.

Resource:

PIP-VPNGW01

Screenshot:

`images/03-public-ip-basic-settings.png`

---

## Step 2

Applied the required Azure Policy tag.

Environment = Produccion

Screenshot:

`images/04-public-ip-tags.png`

---

## Step 3

Validated the Public IP deployment.

Screenshot:

`images/05-public-ip-review.png`

---

## Step 4

Public IP deployed successfully.

Screenshot:

`images/06-public-ip-created.png`

---

## Step 5

Created the mandatory GatewaySubnet.

Network:

VNET-LAB01

Subnet:

GatewaySubnet

Address Space:

10.0.255.0/27

Screenshot:

`images/07-gatewaysubnet-configuration.png`

---

## Step 6

GatewaySubnet successfully deployed.

Screenshot:

`images/08-gatewaysubnet-created.png`

---

## Step 7

Configured Azure VPN Gateway.

Resource:

VPNGW-LAB01

Screenshot:

`images/01-vpngateway-basic-settings.png`

---

## Step 8

Applied required tags.

Environment = Produccion

Screenshot:

`images/02-vpngateway-tags.png`

---

## Step 9

Deployment validation completed successfully.

Screenshot:

`images/09-vpngateway-validation-success.png`

---

## Step 10

VPN Gateway deployment completed.

Screenshot:

`images/10-vpngateway-deployment-success.png`

---

## Step 11

VPN Gateway Overview.

Screenshot:

`images/11-vpngateway-overview.png`

---

# Challenge Encountered

The Azure Policy created in Project 12 required all resources to contain:

Environment = Produccion

Azure VPN Gateway automatically creates a Public IP resource during deployment.

The automatic deployment does not propagate custom tags to the Public IP, causing Azure Policy to reject the deployment.

Additionally, the subscription reached the maximum number of allowed Public IP resources.

---

# Resolution

The issue was resolved by:

- Removing Azure Bastion to free one Public IP quota.
- Creating the Public IP manually.
- Applying the required Azure Policy tag.
- Creating the required GatewaySubnet.
- Reusing the existing Public IP during VPN Gateway deployment.

---

# Skills Demonstrated

- Azure Networking
- Azure VPN Gateway
- Virtual Network Gateway
- GatewaySubnet
- Azure Policy
- Public IP Management
- Troubleshooting Azure Deployments
- Resource Dependencies
- Infrastructure Validation

---

# Result

Azure VPN Gateway deployed successfully using an existing Public IP while complying with Azure Policy requirements.