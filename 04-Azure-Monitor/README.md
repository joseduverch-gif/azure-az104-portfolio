\# Proyecto 04 - Azure Monitor



\## Objetivo



Implementar Azure Monitor para supervisar una máquina virtual y generar una alerta automática cuando el uso de CPU supere el 80%.



\---



\## Recursos utilizados



\- Azure Monitor

\- Alert Rule

\- Action Group

\- Máquina Virtual (VM-WIN01)



\---



\## Configuración



\- Recurso supervisado: VM-WIN01

\- Métrica: Percentage CPU

\- Umbral: 80%

\- Tipo de umbral: Estático

\- Frecuencia de evaluación: 1 minuto

\- Período de retrospectiva: 5 minutos



\---



\## Evidencias



\### Azure Monitor



!\[Monitor](images/monitor-overview.png)



\### Regla de alerta



!\[Alert Rule](images/alert-rule-list.png)



\### Condición de CPU



!\[CPU Condition](images/cpu-condition.png)



\### Action Group



!\[Action Group](images/action-group.png)



\### Detalles de la alerta



!\[Alert Details](images/alert-details.png)



\---



\## Conceptos aprendidos



\- Azure Monitor

\- Alert Rules

\- Métricas

\- Action Groups

\- Supervisión de máquinas virtuales

\- Notificaciones automáticas



\---



\## Resultado



Se configuró una regla de alerta para supervisar el uso de CPU de la máquina virtual VM-WIN01. Cuando el consumo supera el umbral definido, Azure Monitor ejecuta un Action Group para generar una notificación.

