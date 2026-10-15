# RFP: Consultoria de Proyectos

**Clientes:** Consultores de Arquitectura de Datos
   - Football-Soccer-Data-Engineering-Project
   - Asteroid-DataEngineering-Project
   - Binance-Data-Engineering-Project

**Contacto:** [nombre del cliente que firma]

**Equipo redactor:**
Caballero Garcia Yessica Lizeth
Tapia Ledesma Angel Hazel
Sanchez Mayen Tristan Qesen
Sandoval Hernandez Darinka
Salgado Cruz Emiliano Roman

**Fecha de publicación:** [08/10/2026]

## 1. Quiénes somos
Somos un consorcio de operaciones de alto rendimiento que abarca tres sectores críticos: finanzas cuantitativas, divulgación científica y análisis deportivo a nivel internacional. Nuestro negocio principal en estas áreas depende enteramente de la ingesta, procesamiento y explotación de grandes volúmenes de datos para mantener una ventaja competitiva, educar al público y ganar campeonatos mundiales. 

## 2. El problema
Los tres proyectos actuales (análisis de fútbol, rastreo de asteroides y monitoreo financiero en Binance) cuentan con implementaciones funcionales para la extracción de datos, pero presentan áreas de oportunidad significativas en sus arquitecturas. Actualmente, nos duele la falta de estandarización en los procesos de ingesta (ETL/ELT), la ausencia de orquestación automatizada y posibles vulnerabilidades en la gestión de configuraciones. Si no resolvemos esto y optimizamos la infraestructura, los proyectos sufrirán de cuellos de botella al procesar mayores volúmenes de datos, serán difíciles de mantener o escalar, y correrán el riesgo de tener inconsistencias o caídas silenciosas en el flujo de información.

## 3. Qué necesitamos lograr
| # | Necesidad | Cómo sabremos que se cumplió (medible) |
|---|---|---|
| N1 | Estandarización y modernización de la arquitectura de datos. | Entrega de diagramas de arquitectura unificados (As-Is y To-Be) validando el flujo desde la API hasta el almacenamiento final. |
| N2 | Optimización e implementación de mejores prácticas en los pipelines de ETL/ELT. | Orquestación funcional de los procesos (ej. mediante Airflow, Mage o Prefect) con logs de ejecución y monitoreo de errores. |
| N3 | Mejora en las prácticas de despliegue y portabilidad de los entornos. | Proyectos 100% contenerizados con Docker / Docker Compose que se ejecuten exitosamente con un solo comando. |
| N4 | Aseguramiento de la calidad de los datos y gobernanza. | Implementación de validaciones de esquema (ej. Great Expectations o Pydantic) y cero credenciales expuestas en repositorios. |


## 4. Qué NO queremos en este proyecto
- No queremos el desarrollo desde cero de nuevos pipelines; se debe trabajar sobre el código e ideas base existentes.
- No buscamos la creación de modelos de Machine Learning ni Dashboards complejos (el foco es estrictamente la Ingeniería de Datos).
- No aceptaremos arquitecturas que dependan de software propietario o licencias costosas; priorizamos herramientas Open Source.

## 5. Datos que tenemos y datos que faltan
**Qué tenemos:** Contamos con el código fuente base alojado en GitHub, acceso documentado a las APIs de origen (Binance, NASA, APIs de Futbol) y un entendimiento claro de los objetivos de negocio de cada flujo.
**Qué falta:** Nos falta documentar los volúmenes de datos máximos proyectados, definir el esquema de bases de datos definitivo y establecer un modelo formal de recuperación ante desastres o fallos en las APIs origen.


## 6. Restricciones
- **Presupuesto máximo:** Costo operativo unificado enfocado en el modelo de pago por uso (Serverless) de AWS.
- **Plazo:** 10 semanas para refactorizar los 3 ecosistemas y estabilizar la nueva arquitectura en producción.
- **Costo de operación:**
  
1. Arquitecto Cloud (AWS): $75,000 MXN / mes (Reemplazará EC2 por Lambda/EventBridge).


2. Data Engineers (PySpark): $100,000 MXN / mes en total (Unificarán los particionamientos a year=month= y crearán las reglas de Data Quality para desviar fallos).


- Project Manager: $45,000 MXN / mes.
Costo de producción (talento): $550,000 MXN

- Argumento de Venta (El Retorno de Inversión para el Cliente): Al unificar la arquitectura, el cliente ahorrará mes con mes al eliminar la instancia unam-2026-ingenieriadedatos-grupo6 y optimizar el escaneo de Amazon Athena en el proyecto de fútbol (al refinar las particiones). El costo operativo unificado en la nube para todo el consorcio caerá drásticamente.

- Precio Total para el Cliente:

Costo Base: $550,000 MXN

Margen Comercial (45% para la consultora): $450,000 MXN
**TOTAL A COBRAR: $1,000,000 MXN + IVA**


- **Seguridad y privacidad:** Aislamiento estricto de accesos. El rol que procesa los KPIs de fútbol (como efectividad y goles) no debe tener visibilidad sobre las señales de STRONG BUY de criptomonedas ni sobre la energía de megatones simulada en Defensa Planetaria.
- **Quien lo va a usar:** Analistas de datos, científicos espaciales y operadores financieros mediante las vistas estructuradas en Amazon Athena.



## 7. Qué esperamos recibir
- Un reporte de auditoría técnica por cada repositorio identificando antipatrones y deuda técnica.
- Una propuesta de rediseño arquitectónico (diagramas de flujo y de red) enfocada en escalabilidad y resiliencia.
- El código refactorizado y contenerizado que implemente pipelines automatizados, modulares y tolerantes a fallos.
- Documentación técnica detallada (ReadMe robusto, guías de despliegue local y en la nube).


## 8. Cómo evaluaremos las propuestas
| Criterio | Peso (suma 100) |
|---|---|
| Robustez y escalabilidad de la arquitectura propuesta | 40 |
| Uso eficiente de herramientas Open Source y bajo costo operativo | 30 |
| Calidad del código, uso de contenedores (Docker) y automatización | 20 |
| Claridad de la documentación y manejo de riesgos (seguridad) | 10 |

## 9. Qué debe incluir su propuesta
La propuesta debe incluir un *Statement of Work* (SOW) detallando el alcance de las refactorizaciones, un calendario semanal con hitos de entrega (Gantt), diagramas de arquitectura propuestos para cada uno de los tres entornos, el stack tecnológico que recomiendan implementar, y una matriz con al menos tres riesgos técnicos y su plan de mitigación.

## 10. Calendario del proceso
- Fecha límite para preguntas: 15/10/2026
- Fecha límite para entregar propuestas: 22/10/2026
- Fecha de decisión: 26/10/2026
