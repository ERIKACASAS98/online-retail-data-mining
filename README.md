# Online Retail II - Data Mining

Proyecto de minería de datos aplicado al conjunto **Online Retail II**, con el objetivo de analizar el comportamiento de los clientes y descubrir patrones de compra frecuentes.

## Objetivos

El análisis busca responder principalmente dos preguntas:

- ¿Qué grupos de clientes existen y cómo debería tratarse comercialmente cada uno?
- ¿Qué productos se compran juntos con una frecuencia mayor a la esperada?

## Dataset

Se utilizó el conjunto de datos **Online Retail II**, correspondiente a transacciones de una tienda online del Reino Unido.

Fuente: Kaggle / UCI Machine Learning Repository.

## Metodología

El proyecto se desarrolló en tres etapas principales:

1. **Limpieza y preparación de datos**
   - Eliminación de duplicados.
   - Tratamiento de valores faltantes.
   - Exclusión de facturas anuladas.
   - Eliminación de registros con precios o cantidades no válidas.
   - Filtrado de códigos que no corresponden a productos.

2. **Segmentación de clientes**
   - Construcción de variables RFM:
     - Recencia.
     - Frecuencia.
     - Monto.
   - Transformación logarítmica.
   - Estandarización.
   - Segmentación mediante **K-means**.
   - Se identificaron 4 grupos de clientes:
     - VIP.
     - Clientes potenciales.
     - Clientes en riesgo.
     - Clientes inactivos o de bajo valor.

3. **Análisis de asociación**
   - Aplicación del algoritmo **Apriori**.
   - Generación de reglas de asociación.
   - Evaluación mediante soporte, confianza y lift.
   - Identificación de productos que suelen comprarse juntos.

## Resultados principales

Después de la limpieza, el conjunto pasó de **1.067.371 registros a 775.543 registros válidos**.

La segmentación mostró que un grupo relativamente pequeño de clientes concentra gran parte de la facturación, mientras que otro grupo amplio presenta baja frecuencia y bajo valor.

También se encontraron asociaciones fuertes entre productos de colecciones similares, lo que permite proponer estrategias de venta cruzada y paquetes de productos.

## Tecnologías utilizadas

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Mlxtend
- KaggleHub
- Google Colab

## Autora

**Erika Casas Toro**

Estudiante de Ingeniería en Analítica de Datos.
