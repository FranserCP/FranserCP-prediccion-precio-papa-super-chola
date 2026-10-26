# Predicción semanal del precio de la papa súper chola

**Proyecto de investigación de maestría | Riobamba, Ecuador**

## 📌 Descripción del proyecto

Este repositorio contiene los códigos en R utilizados para desarrollar un modelo predictivo del precio semanal de la papa súper chola en Riobamba, Ecuador.

La investigación utiliza técnicas de series temporales y aprendizaje automático para analizar el comportamiento histórico de los precios y comparar diferentes modelos predictivos.

## 🎯 Objetivo

Estimar el precio semanal de la papa súper chola mediante modelos estadísticos y algoritmos de aprendizaje automático, identificando el modelo con mejor desempeño predictivo.

## 📊 Modelos implementados

- **Series temporales:** ARIMA, SARIMA, ARIMAX y SARIMAX.
- **Aprendizaje automático:** Random Forest y XGBoost.

Se evaluaron modelos con y sin variables climáticas. El mejor desempeño se obtuvo con **XGBoost utilizando únicamente información histórica de precios**.

## 🏆 Principales resultados

El modelo seleccionado fue **XGBoost semanal sin variables climáticas**, con los siguientes resultados:

| Métrica | Resultado |
|---|---|
| MAE | 0,61 USD/quintal |
| RMSE | 1,04 USD/quintal |
| MAPE | 2,93 % |
| R² | 0,86 |

## 📁 Organización del repositorio

- **`datos/`**: Archivos de datos utilizados en la investigación.
- **`scripts/`**: Códigos en R para el procesamiento, modelado y evaluación.
- **`resultados/`**: Resultados obtenidos durante el análisis.

## 💻 Reproducción del análisis

Para revisar y reproducir el análisis:

1. Descargar o clonar este repositorio.
2. Abrir los archivos de la carpeta `scripts/` en RStudio.
3. Instalar los paquetes de R requeridos por los scripts.
4. Verificar las rutas de los archivos de entrada de `datos/`.
5. Ejecutar los códigos correspondientes al procesamiento y entrenamiento de los modelos.

**Nota:** Las instrucciones detalladas de ejecución y las versiones de las dependencias se documentarán posteriormente.

## 📚 Fuente de información

Los datos de precios utilizados en la investigación provienen del Sistema de Información Pública Agropecuaria (SIPA) de Ecuador.

## 👨‍💻 Autor

**Ronny Cartagena**

Proyecto de investigación desarrollado como parte del trabajo de titulación de maestría.
