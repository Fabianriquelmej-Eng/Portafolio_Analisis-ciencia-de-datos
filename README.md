# Detección de Patrones mediante Machine Learning y Validación Estadística con KPIs Estratégicos

## Resumen
En entornos de alta incertidumbre logística, la gestión de inventarios basada en promedios simples oculta ineficiencias críticas. Este proyecto implementa un sistema de control avanzado que combina Algoritmos de Agrupamiento con una rigurosa Validación Estadística para optimizar la toma de decisiones.

El objetivo central es transformar datos transaccionales en una Matriz de Control Táctico, permitiendo detectar riesgos de obsolescencia y oportunidades de capitalización que no son visibles a simple vista.

---

## Metodología de trabajo
El flujo de trabajo se diseñó para auditar la salud del inventario mediante tres fases de validación:

1.  **Levantamiento y analisis de KPIs (RFM):** Construcción de indicadores de Recencia, Frecuencia y Valor Monetario para medir el desempeño real de cada ítem.
2.  **Normalización Robusta:** Aplicación de `RobustScaler` y transformaciones logarítmicas para mitigar el sesgo de valores atípicos y garantizar la integridad del modelo.
3.  **Detección de Patrones (K-Means):** Segmentación matemática (k=4) validada por el Método del Codo, asegurando la granularidad óptima para la gestión operativa.

---

## Resultados: Matriz de Decisión Táctica
El modelo reveló 4 perfiles de comportamiento diferenciados, cada uno requiriendo un protocolo de control específico.

**(Aquí puedes insertar una imagen de tu Heatmap o Boxplots si lo deseas)**

### Estrategias de Control Asignadas

| Perfil Identificado | Diagnóstico Estadístico | Protocolo de Control |
| :--- | :--- | :--- |
| **Cluster 3: Productos Estrella** | **Alta Rotación (σ=0.17) / Alto Valor.** Patrón de demanda agresivo y predecible. | **Prioridad Crítica:** Monitoreo diario de disponibilidad y pronóstico de demanda de alta precisión ("Zero-Stock-Out"). |
| **Cluster 1: Sostenedores** | **Rotación Constante.** Comportamiento estable que sostiene la base operativa. | **Automatización:** Configuración de reposición automática (ROP) para reducir carga administrativa. |
| **Cluster 2: Estándar** | **Comportamiento Promedio.** Métricas centradas en la media, desempeño moderado. | **Eficiencia:** Revisión periódica de lotes de compra para optimizar costos logísticos. |
| **Cluster 0: Pasivos** | **Alta Recencia / Baja Rotación.** Indicadores de estancamiento y obsolescencia. | **Saneamiento:** Ejecución de estrategias de salida (liquidación/castigo) para liberar Capital de Trabajo. |

---

## Próximos Pasos y Mejora Continua
Para robustecer la toma de decisiones, se han definido dos líneas de investigación futura que profundizarán la granularidad del control:

### 1. Análisis de Correlación Intra-Cluster
El siguiente paso es auditar cómo interactúan las métricas **dentro de cada segmento específico** para detectar si los impulsores de valor en el grupo "Estrella" son los mismos que en el grupo "Estándar".

### 2. Sub-segmentación Supervisada (Decision Trees)
Se implementarán modelos de **Árboles de Decisión** para extraer reglas de negocio explícitas, generando un **Scorecard de Reglas** (Ej: Si X > 5 y Y < 2) aplicable por el equipo operativo sin necesidad de correr el modelo completo.

---


**Por: Fabian Riquelme Jorquera** 
**Ingeniero Industrial // Analista de datos**

