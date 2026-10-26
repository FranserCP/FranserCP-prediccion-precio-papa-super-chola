# 🥔 Predicción semanal del precio de la papa súper chola en Riobamba

**Proyecto de investigación | Maestría en Inteligencia de Negocios y Ciencia de Datos**

**Universidad Indoamérica | Ecuador, 2026**

## 📌 Descripción del proyecto

Este repositorio contiene los scripts desarrollados en R para la predicción del precio semanal de la papa súper chola comercializada en el mercado mayorista de Riobamba, Ecuador.

La investigación compara modelos estadísticos de series temporales y algoritmos de aprendizaje automático, utilizando registros históricos de precios y variables climáticas para identificar la alternativa con mejor desempeño predictivo.

## 🎯 Objetivo

Implementar y comparar modelos de series temporales y aprendizaje automático para estimar el precio semanal de la papa súper chola en Riobamba, con el propósito de aportar información que apoye la toma de decisiones en el sector agrícola.

## 📊 Datos utilizados

- **Precios agrícolas:** Sistema de Información Pública Agropecuaria (SIPA).
- **Variables climáticas:** Meteostat.
- **Período de precios:** enero de 2022 a junio de 2026.
- **Registros originales de precios:** 628 observaciones.
- **Frecuencia de análisis:** semanal.
- **Variables climáticas:** temperatura promedio, precipitación y velocidad del viento.

## 🤖 Modelos implementados

Se evaluaron ocho configuraciones predictivas correspondientes a seis modelos:

**Modelos de series temporales:**
- ARIMA
- SARIMA
- ARIMAX
- SARIMAX

**Modelos de aprendizaje automático:**
- Random Forest (con y sin clima)
- XGBoost (con y sin clima)

## 🏆 Modelo seleccionado: ARIMAX

Después de comparar los modelos mediante las métricas MAE, RMSE, MAPE, sMAPE y R², **ARIMAX obtuvo el mejor desempeño predictivo general**.

Este modelo combina el comportamiento histórico del precio con información climática rezagada una semana.

### Resultados principales

| Métrica | Resultado |
|---|---|
| MAE | 1,56 USD/quintal |
| RMSE | 2,09 USD/quintal |
| MAPE | 7,75 % |
| sMAPE | 7,81 % |
| R² | 0,33 |

Estos resultados corresponden a la evaluación fuera de muestra y muestran que ARIMAX obtuvo el menor error entre las configuraciones analizadas.

## 📁 Organización del repositorio

- **`datos/`**: Bases históricas de precios agrícolas y variables climáticas.
- **`scripts/`**: Códigos R utilizados para el procesamiento, modelado y evaluación.
- **`resultados/`**: Resultados y visualizaciones generadas durante la investigación.

## 💻 Reproducción del análisis

Para revisar y ejecutar los análisis:

1. Descargar el repositorio desde GitHub.
2. Abrir los archivos de la carpeta `scripts/` utilizando RStudio.
3. Instalar los paquetes de R requeridos por cada script.
4. Verificar las rutas de los archivos de entrada ubicados en `datos/`.
5. Ejecutar los scripts de procesamiento y modelado, respetando sus dependencias.
6. Consultar los archivos generados en `resultados/`.

**Nota:** Próximamente se incorporarán instrucciones detalladas de ejecución y las versiones de los paquetes utilizados para facilitar la reproducción completa.

## 📈 Visualización de resultados

La investigación incluye un dashboard interactivo desarrollado en **Looker Studio**, que permite consultar el comportamiento histórico del precio, las métricas de evaluación y las estimaciones del modelo seleccionado.

## 👨‍🎓 Autor

**Ronny Franser Cartagena Peralta**

Maestría en Inteligencia de Negocios y Ciencia de Datos.

**Universidad Indoamérica — 2026**

Trabajo de titulación: *Modelos estadísticos para la predicción del precio de la papa chola en Riobamba*.
