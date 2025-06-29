# Challengue_Alura_LATAM_DataScience_TelecomX
Proyecto de DataScience 
# Análisis de Abandono de Clientes en Telecomunicaciones

Este proyecto realiza un análisis exploratorio de datos para identificar los factores clave que influyen en el abandono de clientes (Churn) en una empresa de telecomunicaciones.

## Datos

El análisis se basa en el conjunto de datos `TelecomX_Data.json`, que contiene información detallada sobre los clientes, incluyendo:

- **customerID**: Identificador único del cliente.
- **Churn**: Indica si el cliente abandonó el servicio (Yes) o no (No).
- **customer**: Información demográfica del cliente (género, si es adulto mayor, si tiene pareja, si tiene dependientes, antigüedad - tenure).
- **phone**: Información sobre el servicio telefónico (si tiene servicio telefónico, si tiene múltiples líneas).
- **internet**: Información sobre el servicio de internet (tipo de servicio, seguridad online, backup online, protección de dispositivo, soporte técnico, streaming de TV, streaming de películas).
- **account**: Información de la cuenta (tipo de contrato, facturación sin papel, método de pago, cargos mensuales, cargos totales).

## Análisis Realizado

El análisis incluye los siguientes pasos:

1.  **Extracción de Datos**: Carga de los datos desde la URL proporcionada y normalización del archivo JSON a un DataFrame plano.
2.  **Transformación de Datos**:
    *   Verificación de la forma y tipos de datos del DataFrame normalizado.
    *   Identificación de columnas importantes para el análisis.
    *   Verificación de valores nulos y duplicados.
    *   Inserción de una nueva columna 'Cuentas_Diarias' calculada a partir de los cargos mensuales.
    *   Conversión de la columna 'account.Charges.Total' a tipo numérico.
    *   Eliminación de filas con valores vacíos en la columna 'Churn'.
3.  **Carga y Análisis Visual**: Generación de visualizaciones para explorar la relación entre diferentes variables y el abandono de clientes, incluyendo:
    *   Abandono por Género.
    *   Tasa de Abandono en Adultos Mayores.
    *   Tiempo (en meses) en el que las personas evaden más (distribución de tenure por churn).
    *   Tasa de Abandono por Antigüedad (Tenure).
    *   Tendencia de cargos mensuales por abandono (Tenure vs Cargos mensuales por Churn).
    *   Abandono por Tipo de Contrato.
    *   Evasión por Valor Total Mensual (Box plot de cargos mensuales por Churn).
    *   Evasión si tiene Servicio Telefónico.
    *   Evasión por Servicio de Internet.
    *   Evasión por Servicio de Streaming (TV).
    *   Evasión por Método de Pago.

## Hallazgos Clave (Basado en las Visualizaciones)

*   **Género**: (Describe brevemente lo que observaste en el gráfico de abandono por género - por ejemplo, si hay una diferencia notable o no).
*   **Adultos Mayores**: (Describe brevemente lo que observaste en el gráfico de adultos mayores - por ejemplo, si los adultos mayores tienen una tasa de abandono mayor o menor).
*   **Antigüedad (Tenure)**: (Resume la tendencia observada en el gráfico de tasa de abandono por tenure - por ejemplo, si la tasa de abandono es mayor en los primeros meses).
*   **Cargos Mensuales**: (Describe la relación entre cargos mensuales y abandono observada en el gráfico de dispersión y el box plot - por ejemplo, si los clientes que abandonan tienden a tener cargos mensuales más altos).
*   **Tipo de Contrato**: (Comenta sobre la influencia del tipo de contrato en el abandono - por ejemplo, si los contratos mes a mes tienen una tasa de abandono más alta).
*   **Servicio Telefónico**: (Describe si el tener servicio telefónico impacta en el abandono).
*   **Servicio de Internet**: (Comenta qué tipo de servicio de internet parece tener una mayor o menor tasa de abandono).
*   **Servicio de Streaming**: (Describe si el servicio de streaming de TV influye en el abandono).
*   **Método de Pago**: (Identifica qué métodos de pago están asociados con tasas de abandono más altas o bajas).

## Cómo Ejecutar el Código

1.  Clona este repositorio.
2.  Abre el notebook de Colab (`nombre_del_notebook.ipynb`).
3.  Ejecuta las celdas en orden.

## Próximos Pasos

*   Realizar análisis estadísticos más profundos (correlaciones, pruebas de hipótesis).
*   Implementar modelos predictivos para predecir el abandono de clientes.
*   Explorar otras variables y combinaciones de variables.
*   Crear un informe más detallado con interpretaciones y recomendaciones.


https://github.com/user-attachments/assets/1e07a9b7-1f6a-4f2a-ae8f-c8e0ec6ae6c5

