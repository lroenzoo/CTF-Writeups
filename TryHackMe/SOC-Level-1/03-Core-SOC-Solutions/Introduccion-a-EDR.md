# Introducción a EDR

## ¿De qué trata?
Fundamentos del EDR (Endpoint Detection and Response), sus diferencias 
con el antivirus tradicional y cómo funciona en un entorno SOC.

## Conceptos clave

### ¿Qué es un EDR?
Solución de seguridad que monitorea y registra continuamente el 
comportamiento de los endpoints para detectar amenazas avanzadas 
que evaden el antivirus tradicional.

### AV vs EDR
| Antivirus (AV) | EDR |
|----------------|-----|
| Detección basada en firmas | Detección basada en comportamiento |
| Lista de amenazas conocidas | Monitoreo continuo de actividad |
| Protección en el punto de entrada | Protección dentro del endpoint |
| No detecta amenazas nuevas | Detecta amenazas desconocidas |

**Analogía:** El AV es el control de pasaportes en un aeropuerto. 
El EDR son los guardias con cámaras dentro del aeropuerto.

### ¿Cómo funciona un EDR?
1. Monitorea continuamente todos los procesos del endpoint
2. Registra la telemetría (logs de actividad)
3. Detecta comportamientos sospechosos
4. Alerta al SOC o toma acción automática

### Telemetría EDR
Datos que recopila el EDR:
- Procesos ejecutados
- Conexiones de red
- Archivos creados/modificados
- Comandos ejecutados (PowerShell, CMD)
- Inyecciones de procesos

### Capacidades de detección y respuesta
- Detección de amenazas avanzadas (APT, fileless malware)
- Correlación de eventos entre endpoints
- Respuesta automática (aislar equipo, matar proceso)
- Visibilidad organizacional completa

## Lab: Investigación de alertas EDR
Investigación de alertas buscando rutas maliciosas y URLs sospechosas 
en los logs del EDR.

### Aprendizaje
El EDR es esencial en un SOC moderno. Donde el AV falla ante ataques 
avanzados (ofuscación, inyección en procesos legítimos), el EDR 
detecta el comportamiento anómalo y permite responder a tiempo.