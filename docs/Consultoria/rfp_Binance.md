# RFP: MarketMatrix - Consultoría en Data Pipeline Financiero

**Cliente: Binance Data Engineering Project**
**Contacto: Dirección de Operaciones y Riesgos**

**Equipo consultor: Consultoría en Ingeniería de Datos TeamThree**
**Fecha de publicación:** [13/10/2026]

## 1. Quiénes somos
Somos una consultoría en ingeniería de datos especializada en infraestructura de datos de alta frecuencia. Presentamos este documento a MarketMatrix, fondo de inversión de trading cuantitativo, para ofrecer nuestros servicios de optimización y estabilización de sus algoritmos de volatilidad de Bitcoin.

## 2. El problema
Nuestro análisis de su arquitectura actual revela una gran inestabilidad en el pipeline de datos que extrae información de Binance y serias deficiencias en la ejecución en la nube de su lógica de triple confirmación (RSI, Bollinger, MACD). Advertimos que esta deuda técnica expone al fondo a pérdidas millonarias; la latencia de procesamiento ante eventos de alta volatilidad está impidiendo que su mesa de control tome decisiones precisas.
Ademas, otro de los problemas al cual nos enfrentamos es hacer que el proyecto sea redituable en cuanto a las ganancias, tanto para la empresa dueña del proyecto como para nosotros como consultora.  

## 3. Qué necesitamos lograr
Como sus consultores, garantizamos la implementación de los siguientes hitos:
| # | Necesidad | Cómo sabremos que se cumplió (medible) |
|---|---|---|
| N1 | Estabilización del Data Lakehouse | Entregaremos un pipeline orquestado con AWS Lambda y EventBridge que opere de forma desatendida y sin caídas. |
| N2 | Escalabilidad ante alta frecuencia | Configuraremos una arquitectura elástica que asimile ráfagas bruscas de datos del mercado sin degradar el tiempo de respuesta. |
| N3 | Protección del capital | Expondremos vistas materializadas en Athena que brinden señales instantáneas de COMPRA/VENTA a sus algoritmos. |

## 4. Qué NO queremos en este proyecto
Como consoltora enfocada en Cloud, excluimos de nuestra propuesta el uso de herramientas de código abierto autogestionadas. Además, garantizamos que no implementaremos servidores virtuales (como Amazon EC2) para evitarles costos por infraestructura inactiva.

## 5. Datos que tenemos y datos que faltan
Partiremos de la extracción cruda de las velas de cierre (Klines) en CSV y las transformaciones iniciales que su equipo ya posee. Nosotros aportaremos el desarrollo faltante: la orquestación profesional en AWS Glue y la capa de exposición optimizada para su sistema de trading.

## 6. Restricciones
* **Presupuesto máximo:** Nuestro esquema de cobro se adapta a su límite de $550,000 MXN por el proyecto completo.
* **Plazo:** Nos comprometemos a liberar el proyecto en 10 semanas.
* **Seguridad y privacidad:** Diseñaremos los permisos aplicando el Principio de Mínimo Privilegio (IAM) para aislar sus buckets de S3.
* **Quien lo va a usar:** Los datos procesados serán consumidos por sus sistemas de trading algorítmico y su mesa de control.

## 7. Qué esperamos recibir
(Enfoque de la consultora: Qué entregaremos al cliente).
Otorgaremos una reingeniería profunda de su ecosistema, volviéndolo 100% nativo en AWS. Recibirán infraestructura como código, scripts de PySpark en AWS Glue totalmente optimizados, y documentación operativa para sus ingenieros.

## 8. Cómo evaluaremos las propuestas
(Enfoque de la consultora: Nuestra propuesta de valor frente a sus criterios).
Nuestra solución responde a sus exigencias porque ofrecemos:
* 40%: Especialización exclusiva y certificada en servicios nativos de AWS.
* 30%: Arquitecturas diseñadas específicamente para la mitigación de riesgos financieros en alta frecuencia.
* 20%: Optimización de recursos para no superar el presupuesto asignado.
* 10%: Entregas modulares comprobables en el plazo acordado.

## 9. Qué debe incluir su propuesta
(Enfoque de la consultora: Estructura de nuestra intervención).
Asignaremos un equipo técnico de alto rendimiento (Data Engineers y Lead Data Engineer) dedicados al diseño y despliegue en AWS, estructurando el avance en fases de entrega bisemanales.