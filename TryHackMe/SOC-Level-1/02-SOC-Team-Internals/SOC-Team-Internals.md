# SOC Team Internals

## ¿De qué trata?
Exploración de las habilidades esenciales de un analista SOC para 
clasificar, priorizar y escalar alertas en entornos reales.

## Conceptos clave

### ¿Qué es una alerta?
Una notificación generada por herramientas de seguridad (como un SIEM)
cuando se detecta actividad sospechosa o que viola una regla definida.

### Función del L1 en la clasificación de alertas
- Primera línea de respuesta
- Recibe y revisa las alertas entrantes
- Determina si es True Positive o False Positive
- Escala al L2 cuando el incidente lo requiere

### Propiedades de una alerta
- **Severidad:** Critical, High, Medium, Low
- **Status:** New, In Progress, Closed
- **Veredicto:** True Positive, False Positive
- **Assignee:** analista responsable

### Priorización de alertas
Las alertas se priorizan según su severidad:
1. Critical
2. High
3. Medium
4. Low

### Triaje de alertas
Proceso de revisar, clasificar y tomar acción sobre una alerta:
1. Revisar los detalles de la alerta
2. Analizar el contexto (usuario, IP, red, archivo)
3. Determinar si es True Positive o False Positive
4. Comentar con el análisis realizado
5. Cerrar o escalar según corresponda

## Lab: Alert Triage - SOC L1 Simulator

Simulación de triaje de alertas reales en una plataforma SOC.

| Alerta | Severidad | Veredicto | Razonamiento |
|--------|-----------|-----------|--------------|
| Potential Data Exfiltration | Critical | False Positive | Tráfico hacia *.zoom.us desde sala de reuniones, actividad legítima |
| Double-Extension File Creation | High | True Positive | Archivo cats2025.mp4.exe descargado desde dominio sospechoso |
| Download from GitHub Repository | Low | False Positive | Desarrollador de VPN/DEVELOPERS descargando React, actividad legítima |

## Aprendizaje
El triaje efectivo requiere analizar el contexto completo de la alerta,
no solo la severidad. Una alerta Critical puede ser False Positive y una
Low puede ser True Positive. El analista L1 debe saber cuándo cerrar
y cuándo escalar.