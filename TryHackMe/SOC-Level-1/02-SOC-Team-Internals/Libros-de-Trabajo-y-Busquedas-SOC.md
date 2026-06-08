# Libros de Trabajo y Búsquedas de SOC

## ¿De qué trata?
Recursos corporativos que ayudan al analista SOC L1 a estructurar 
y simplificar la clasificación de alertas mediante flujos de trabajo 
estandarizados.

## Conceptos clave

### Inventario de Identidades
Catálogo de empleados y cuentas de usuario de la organización.
Permite al analista obtener contexto sobre quién está involucrado 
en una alerta (rol, departamento, accesos esperados).

Fuentes comunes:
- Active Directory / Entra ID
- SSO Providers (Okta, Google Workspace)
- HR Systems (BambooHR, SAP)
- Soluciones personalizadas (CSV, Excel)

### Inventario de Activos
Lista de todos los servidores y estaciones de trabajo del entorno IT.
Permite entender qué hace cada sistema y quién puede acceder a él.

Fuentes comunes:
- Active Directory
- SIEM o EDR (Elastic, CrowdStrike)
- MDM Solutions (MS Intune, Jamf)
- Soluciones personalizadas (CSV, Excel)

### Diagramas de Red
Representación visual de la infraestructura de red que ayuda 
al analista a entender el flujo del tráfico y ubicar los activos.

### Cuadernos de Ejercicios (Workbooks)
Flujos de decisión paso a paso que guían al analista L1 durante 
el triaje de una alerta. Estandarizan el proceso y reducen errores.

## Lab: Workbook de Análisis de Email de Phishing

Flujo completado para analizar una alerta de email de phishing:

1. Investigar el email con EML analyser (SPF/DKIM, contenido, reputación del dominio)
2. Tomar ownership de la alerta y usar el inventario de identidades para contextualizar destinatarios
3. Recolectar evidencia de triaje (lista de destinatarios, reporte sandbox, resultados EML)
4. **Decisión:** ¿El adjunto es malicioso, el origen es falso o el email es inesperado?
   - **SÍ** → Escribir reporte para L2 con evidencia → Escalar a L2
   - **NO** → Escribir comentario explicando por qué es seguro → Cerrar como FP

## Aprendizaje
Los workbooks y los inventarios son herramientas fundamentales del SOC.
Permiten al L1 tomar decisiones consistentes y documentadas, 
sin depender solo del criterio personal.