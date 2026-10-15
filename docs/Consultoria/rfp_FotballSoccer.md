# RFP: Sistema de Analítica de Fútbol - Propuesta de Migración a la Nube

**Cliente: Football Soccer Data Engineering Project**
**Contacto: Dirección de Selecciones Nacionales**+

**Equipo consultor: Consultoría en Ingeniería de Datos TeamThree**
**Fecha de publicación:** [13/10/2026]

## 1. Quiénes somos
Somos una consultora especializada en arquitecturas de datos Serverless y optimización de costos cloud. Presentamos esta propuesta técnica a la Dirección de Selecciones Nacionales para revolucionar la forma en que procesan la inteligencia deportiva (la cual se presentó para la Copa Mundial de la FIFA 2026 pero se extendera para otros eventos deportivos).

## 2. El problema
Nuestro diagnóstico de su sistema actual revela una severa ineficiencia: están pagando facturas de AWS infladas por tener una instancia de servidor virtual para extraer datos históricos, acoplado a un bucket con particionamiento ineficiente (solo por año). Como consultores, sabemos que esto provoca consultas lentas que impiden al cuerpo técnico tomar decisiones estratégicas de forma ágil, haciéndoles perder ventaja táctica frente a otras selecciones.
Ademas, otro de los problemas al cual nos enfrentamos es hacer que el proyecto sea redituable en cuanto a las ganancias, tanto para la empresa dueña del proyecto como para nosotros como consultora.

## 3. Qué necesitamos lograr
Nuestra intervención técnica garantizará lo siguiente:
| # | Necesidad | Cómo sabremos que se cumplió (medible) |
|---|---|---|
| N1 | Migración Serverless | Desmantelaremos la instancia EC2 y migraremos los procesos de extracción a AWS Lambda. |
| N2 | Optimización de Consultas Analíticas | Reprocesaremos la capa Silver aplicando un particionamiento eficiente bajo formato Parquet. |
| N3 | Inteligencia Deportiva | Entregaremos vistas en Amazon Athena listas para calcular KPIs (efectividad, goles) para el cuerpo técnico. |

## 4. Qué NO queremos en este proyecto
Como expertos en optimización Cloud, garantizamos que no utilizaremos servidores virtuales aprovisionados (EC2) para eliminar sus costos por inactividad. Toda la arquitectura se basará estrictamente en el ecosistema nativo de AWS, sin software externo de licenciamiento oculto.

## 5. Datos que tenemos y datos que faltan
Tomaremos como base sus scripts funcionales en Python que consumen la API-Football. Nuestro equipo se encargará de reescribir esta ingesta hacia un modelo nativo y refinar los datos hasta la capa Gold para que ustedes puedan ejecutar análisis avanzados.

## 6. Restricciones
* **Presupuesto máximo:** El costo total de nuestra intervención no excederá los $550,000 MXN.
* **Plazo:** Ejecutaremos la refactorización en 10 semanas para integrarnos a su calendario de preparación.
* **Seguridad y privacidad:** Estableceremos cifrado avanzado y controles IAM estrictos para asegurar la confidencialidad de sus tácticas de scouting.
* **Quien lo va a usar:** Diseñaremos la salida de datos para la interfaz de consumo de su cuerpo técnico y analistas.

## 7. Qué esperamos recibir
(Enfoque de la consultora: Qué entregaremos al cliente).
Proporcionaremos una modernización de infraestructura que reducirá drásticamente sus costos mensuales mediante un enfoque Serverless. Entregaremos despliegues automatizados, bases de datos rápidas y la documentación completa.

## 8. Cómo evaluaremos las propuestas
(Enfoque de la consultora: Nuestra propuesta de valor frente a sus criterios).
Aseguramos el éxito del proyecto porque nuestra consultora aporta:
* 40%: Experiencia técnica comprobable eliminando deuda técnica y modernizando flujos en AWS.
* 30%: Enfoque agresivo en la reducción de costos operativos en la nube (ETL y analítica).
* 20%: Garantía de ejecución sin desviaciones sobre su límite presupuestal.
* 10%: Cumplimiento milimétrico del cronograma de 10 semanas.

## 9. Qué debe incluir su propuesta
(Enfoque de la consultora: Estructura de nuestra intervención).
Proponemos un equipo conformado por 1 Lead Data Engineer y 2 Data Engineers, maximizando su inversión directamente en el código de AWS y omitiendo cargos por roles administrativos (PM) para mantenernos dentro del presupuesto establecido de 2.5 meses. Adjuntaremos los diagramas de arquitectura actualizados.