# Informes de Alertas SOC L1

## ¿De qué trata?
Cómo documentar, escalar y comunicar correctamente las alertas 
de alto riesgo como analista SOC L1.

## Conceptos clave

### Embudo de alerta
Proceso por el cual una alerta pasa por distintas etapas:
recepción → análisis → clasificación → acción (cerrar o escalar)

### Las cinco W para reportes
Framework estándar para documentar incidentes:
- **Who:** ¿Quién está involucrado?
- **What:** ¿Qué ocurrió?
- **When:** ¿Cuándo ocurrió?
- **Where:** ¿Dónde ocurrió?
- **Why:** ¿Por qué es sospechoso?

### Guía de escalamiento
El L1 escala al L2 cuando:
- El incidente requiere análisis más profundo
- Está fuera del alcance del L1
- La severidad es Critical o el impacto es alto

### Comunicación SOC
La comunicación clara y estructurada entre niveles es clave
para una respuesta efectiva a incidentes.

## Lab: Alert Reporting

| Alerta | Severidad | Acción tomada |
|--------|-----------|---------------|
| Email Marked as Phishing after Delivery | Medium | Escalada a L2 (E.Fleming) |

### Aprendizaje
No todas las alertas las resuelve el L1. Saber cuándo escalar 
es tan importante como saber analizar. Un correo de phishing 
requiere análisis profundo de L2.