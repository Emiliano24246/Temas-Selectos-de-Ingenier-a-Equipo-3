# RFP: NEO Risk Monitor - Propuesta de Modernización de Datos

**Cliente: Asteroid DataEngineering Project**
**Contacto: Dirección General de Exposiciones**

**Equipo consultor: [Nombre de tu Consultoría / Equipo]**
**Fecha de publicación:** [13/10/2026]

## 1. Quiénes somos
Somos una consultoría especializada en arquitectura Cloud e Ingeniería de Datos. Nos dirigimos a su red de museos y planetarios con el objetivo de fungir como su brazo tecnológico, ayudándolos a transformar los datos astronómicos de los asteroides (NEOs) en exhibiciones totalmente automatizadas, interactivas y atractivas para su público.

## 2. El problema
Tras revisar la infraestructura del proyecto original, nuestro equipo de consultores detectó una dependencia al procesamiento manual del JSON crudo (con más de 300 campos) proveniente de la API NeoWs de la NASA. Como consultores, entendemos que para su dirección esto se traduce en altos costos por requerir personal especializado para tareas repetitivas, y una pérdida de "engagement" en sus museos debido a que sus pantallas no muestran datos en tiempo real.
Ademas, otro de los problemas al cual nos enfrentamos es hacer que el proyecto sea redituable en cuanto a las ganancias, tanto para la empresa dueña del proyecto como para nosotros como consultora.  

## 3. Qué necesitamos lograr
Nuestra consultoría se compromete a entregar las siguientes soluciones:
| # | Necesidad | Cómo sabremos que se cumplió (medible) |
|---|---|---|
| N1 | Pipeline automatizado en AWS | Entregaremos un flujo donde los datos JSON pasen a formato Parquet en S3 usando AWS Lambda y Glue diariamente, sin intervención humana. |
| N2 | Calidad de Datos (Data Quality) | Programaremos validaciones que rechacen nulos y desvíen errores automáticamente a una ruta de cuarentena en S3. |
| N3 | Generación de métricas para exhibición | Crearemos las tablas en Athena para que sus sistemas consulten el "Risk Score" y la energía de impacto al instante. |

## 4. Qué NO queremos en este proyecto
En nuestra arquitectura propuesta no incluiremos ninguna herramienta, base de datos o servicio de terceros que quede fuera del ecosistema nativo de AWS. Tampoco entregaremos sistemas que requieran mantenimiento o ejecución manual de sus actualizaciones diarias.

## 5. Datos que tenemos y datos que faltan
Sabemos que ustedes ya cuentan con el acceso a la API gratuita de la NASA. Lo que nuestra consultoría aportará es la infraestructura ETL faltante para automatizar la limpieza y el cálculo matemático de las métricas de riesgo que alimentarán sus pantallas interactivas.

## 6. Restricciones
* **Presupuesto máximo:** Nos ajustaremos a su tope de $450,000 MXN para el desarrollo integral.
* **Plazo:** Ejecutaremos el proyecto alineados a su calendario de nuevas exhibiciones.
* **Seguridad y privacidad:** Implementaremos un catálogo gestionado en AWS Glue con controles IAM estrictos.
* **Quien lo va a usar:** Entregaremos un backend optimizado para conectar con los tableros de visualización de su público.

## 7. Qué esperamos recibir
(Enfoque de la consultora: Qué entregaremos al cliente).
Les entregaremos un pipeline Medallón (Bronze, Silver, Gold) "llave en mano", 100% serverless en AWS. Les proporcionaremos toda la documentación y la automatización necesaria para que su red de museos opere esto sin necesidad de contratar un equipo interno de ingeniería.

## 8. Cómo evaluaremos las propuestas
(Enfoque de la consultora: Nuestra propuesta de valor frente a sus criterios).
Nuestra firma cumple con sus criterios de evaluación al garantizar:
* 40%: Certificación y dominio absoluto del ecosistema AWS.
* 30%: Diseño eficiente y probado de arquitecturas Medallón.
* 20%: Transparencia y ajuste total al presupuesto de inversión del museo.
* 10%: Entregas ágiles y en los tiempos estipulados.

## 9. Qué debe incluir su propuesta
(Enfoque de la consultora: Estructura de nuestra intervención).
Nuestra ejecución técnica será liderada por perfiles altamente capacitados, enfocados exclusivamente en la construcción en AWS, con un plan de trabajo iterativo que detallaremos en las mesas de arranque.