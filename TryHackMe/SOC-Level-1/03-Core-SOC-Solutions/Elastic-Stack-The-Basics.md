# Elastic Stack: The Basics

## ¿De qué trata?
Introducción al Elastic Stack (ELK) como alternativa a Splunk,
y uso de KQL (Kibana Query Language) para búsqueda de eventos.

## Conceptos clave

### ¿Qué es Elastic Stack (ELK)?
Conjunto de herramientas open source para recolección,
almacenamiento y visualización de logs:
- **Elasticsearch:** motor de búsqueda y almacenamiento
- **Logstash:** ingesta y procesamiento de logs
- **Kibana:** interfaz visual para búsquedas y dashboards
- **Beats:** agentes livianos que envían logs

### KQL (Kibana Query Language)
Lenguaje de búsqueda de Kibana, más simple que SPL de Splunk.

Operadores básicos:
- **AND:** ambas condiciones deben cumplirse
- **OR:** al menos una condición debe cumplirse
- **NOT:** excluir resultados que cumplan la condición

Ejemplo:
## Lab: Búsqueda con KQL en AttackBox
- Uso de máquina virtual AttackBox
- Búsquedas con AND, OR y NOT en Kibana

## Aprendizaje
Elastic Stack es una alternativa open source muy popular a Splunk.
Conocer ambas herramientas amplía las posibilidades laborales
de un analista SOC.