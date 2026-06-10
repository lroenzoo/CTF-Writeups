# Introducción a SIEM

## ¿De qué trata?
Fundamentos del SIEM (Security Information and Event Management),
por qué es esencial en un SOC y cómo procesa los logs para generar alertas.

## Conceptos clave

### El problema: registros por todas partes
Los sistemas generan logs constantemente desde múltiples fuentes
(firewalls, endpoints, emails, servidores). Sin centralización,
es imposible correlacionar eventos y detectar amenazas.

### ¿Por qué SIEM?
- Centraliza todos los logs en un solo lugar
- Correlaciona eventos de distintas fuentes
- Genera alertas cuando se cumplen reglas predefinidas
- Permite búsquedas e investigaciones rápidas

### Fuentes de registro e ingesta
Fuentes comunes que alimentan un SIEM:
- Firewall
- Endpoints (EDR)
- Correo electrónico
- Servidores web
- Active Directory
- Aplicaciones internas

### Proceso de alerta y análisis
1. Los logs llegan al SIEM desde múltiples fuentes
2. El SIEM aplica reglas de correlación
3. Si los eventos coinciden con una regla, se genera una alerta
4. El analista L1 investiga la alerta en el panel del SIEM

## Lab: Panel de control y eventos
Se activó una alerta porque varios eventos coincidieron con
una regla previamente configurada en el SIEM.

## Aprendizaje
El SIEM es el centro neurálgico del SOC. Sin él, detectar una
amenaza que abarca múltiples sistemas sería casi imposible.