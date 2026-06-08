# Métricas y Objetivos del SOC

## ¿De qué trata?
Exploración de las métricas clave que miden la eficacia de un SOC
y cómo mejorarlas cuando presentan problemas.

## Conceptos clave

### Métricas básicas
Indicadores generales del rendimiento del SOC.

### Métricas de triaje
- **Time to Detect (TTD):** tiempo desde que ocurre el ataque hasta que se genera la alerta
- **Time to Acknowledge (TTA):** tiempo desde que aparece la alerta hasta que el analista la toma
- **Time to Respond (TTR):** tiempo desde el acknowledge hasta que se contiene el incidente
- **False Positive Rate:** porcentaje de alertas que resultan ser actividad legítima

### Mejorar las métricas
Cada métrica tiene un responsable y una solución específica:
- TTD alto → tunear el SIEM para detectar más frecuentemente → SOC Engineer
- TTA alto → mejorar el sistema de notificaciones → SOC Engineer
- TTR alto → crear workbooks con pasos de respuesta → L2
- False Positive Rate alta → excluir ruido del sistema de las reglas → SOC Engineer

## Lab: Request From MDR Top Management

Tres escenarios donde había que identificar la métrica problemática,
la tarea de mejora y el responsable:

| Escenario | Métrica problemática | Mejora | Responsable |
|-----------|---------------------|--------|-------------|
| Cliente insatisfecho (CFO hackeado, 6hs de respuesta) | Time to Respond muy alto | Crear workbook de rotación de credenciales | L2 que manejó el incidente |
| Alerta retrasada (20 min sin alertas en demo) | Time to Detect muy alto | Tunear SIEM para correr cada 5 minutos | SOC Engineer |
| Analistas agotados (95% falsos positivos) | False Positive Rate muy alta | Implementar proceso de remediación de FP | SOC Engineers |

## Aprendizaje
Las métricas del SOC permiten identificar dónde está el problema
y a quién asignárselo. No todas las mejoras las hace el L1,
cada problema tiene el rol correcto para resolverlo.