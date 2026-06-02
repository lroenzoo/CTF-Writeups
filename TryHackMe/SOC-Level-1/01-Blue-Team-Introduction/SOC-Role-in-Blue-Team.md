# SOC Role in Blue Team

## ¿De qué trata?
Introducción a los roles dentro de un SOC y cómo cada uno contribuye 
a la seguridad defensiva.

## Roles del SOC

| Rol | Responsabilidad |
|-----|----------------|
| SOC L1 Analyst | Triage de alertas del SIEM |
| SOC L2 Analyst | Análisis profundo de incidentes |
| SOC Engineer | Mantenimiento de infraestructura y respuesta técnica |
| GRC Auditor | Auditorías de compliance (ej: PCI DSS) |
| CERT Lead | Respuesta inmediata a incidentes críticos |
| Penetration Tester | Búsqueda de vulnerabilidades en sistemas |
| Threat Researcher | Análisis de grupos de amenazas y sus tácticas |

## Conceptos clave
- El SOC es el centro de operaciones de seguridad defensiva
- Cada rol tiene responsabilidades específicas según el tipo de incidente
- El L1 escala al L2 cuando el incidente requiere análisis más profundo

## Lab: TrySecureMe

Ejercicio de asignación de roles a escenarios de seguridad reales.

| Escenario | Rol asignado |
|-----------|-------------|
| Alerta de brute-force en firewall (SIEM) | Lucas - SOC L1 Analyst |
| Análisis profundo de phishing malware | Susan - SOC L2 Analyst |
| Respuesta inmediata a ransomware | Robert - CERT Lead |
| Auditoría PCI DSS de servidores | Nick - GRC Auditor |
| Búsqueda de vulnerabilidades en sitio web | Ben - Penetration Tester |
| Investigación de problema de almacenamiento en SIEM | Eugen - SOC Engineer |
| Análisis de tácticas del grupo FIN7 | Alice - Threat Researcher |

### Aprendizaje
Cada incidente requiere un rol específico según su naturaleza. 
El L1 hace triage, el L2 profundiza, el CERT responde a crisis, 
el GRC audita compliance, y los especialistas (Pen Tester, Threat Researcher) 
cubren áreas técnicas específicas.