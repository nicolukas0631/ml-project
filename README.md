# README for Predictive Modeling Project for OilyGiant

## Overview
This project aims to develop a predictive model for OilyGiant, an oil company seeking to identify the best regions for opening new oil extraction wells. The analysis is based on three different datasets representing various regions, focusing on the volume of reserves per well and other relevant characteristics.

## Objectives
1. Collect parameters and objectives from the different regions.
2. Construct a model to predict the volume of oil reserves in new wells.
3. Select the region with the highest estimated values.
4. Identify the region with the greatest profit potential and the lowest risk of loss.

## Methodology
The project is structured as follows:

1. **Data Preprocessing**: 
   - The datasets were examined for duplicates and null values, confirming that they were in good condition for analysis.
   - Relevant features (`f0`, `f1`, `f2`, and `product`) were selected for modeling.

2. **Modeling**:
   - A linear regression model was built for each region using a training-validation split of 75:25.
   - Features were standardized to improve model performance.
   - The model's performance was evaluated using metrics such as Root Mean Squared Error (RMSE) and R².

3. **Profit Calculation**:
   - The minimum production volume required to avoid losses was established.
   - Potential profits were calculated for the top 200 wells in each region based on predicted volumes.

4. **Risk Analysis**:
   - Bootstrapping techniques were employed to assess the risk of loss and the distribution of potential profits across different regions.

## Conclusions
1. The data preprocessing confirmed that all datasets were clean and ready for analysis.
2. The linear regression model for Region 2 yielded the best performance, with the lowest RMSE and highest R².
3. Despite Region 1 showing the highest potential profits, Region 2 was identified as the best option for development due to its favorable risk-to-reward ratio, with an average profit of $4.5 million and a loss risk of only 1.5%.

This project provides valuable insights for OilyGiant in making informed decisions regarding oil extraction investments.


# Proyecto de Modelado Predictivo para OilyGiant / Predictive Modeling Project for OilyGiant

---

## Español

### Descripción General
Este proyecto desarrolla un modelo predictivo para OilyGiant, una empresa petrolera que busca identificar la mejor región para abrir nuevos pozos de extracción. El análisis se basa en tres conjuntos de datos de diferentes regiones, considerando el volumen de reservas por pozo y otras características relevantes.

### Objetivos
1. Recopilar parámetros y objetivos de las diferentes regiones.
2. Construir un modelo para predecir el volumen de reservas de petróleo en nuevos pozos.
3. Seleccionar la región con los valores estimados más altos.
4. Identificar la región con mayor potencial de beneficio y menor riesgo de pérdida.

### Metodología
- **Preprocesamiento de Datos**: Se verificó la ausencia de duplicados y valores nulos. Se seleccionaron las variables `f0`, `f1`, `f2` y `product`.
- **Modelado**: Se entrenó un modelo de regresión lineal para cada región, dividiendo los datos en entrenamiento y validación (75:25) y estandarizando las características. Se evaluó el desempeño con RECM y R².
- **Cálculo de Ganancias**: Se estableció el volumen mínimo necesario para evitar pérdidas y se calcularon las ganancias potenciales para los 200 mejores pozos de cada región.
- **Análisis de Riesgo**: Se utilizó bootstrapping para estimar el riesgo de pérdida y la distribución de ganancias.

### Conclusiones
- Los datos estaban limpios y listos para el análisis.
- El modelo de la Región 2 tuvo el mejor desempeño (menor RECM y mayor R²).
- Aunque la Región 1 mostró mayores ganancias potenciales, la Región 2 es la mejor opción por su bajo riesgo (1.5%) y ganancia promedio de $4.5 millones.

---

## English

### Overview
This project develops a predictive model for OilyGiant, an oil company seeking to identify the best region to open new extraction wells. The analysis is based on three datasets from different regions, focusing on the volume of reserves per well and other relevant features.

### Objectives
1. Collect parameters and objectives from different regions.
2. Build a model to predict oil reserve volumes in new wells.
3. Select the region with the highest estimated values.
4. Identify the region with the greatest profit potential and lowest risk of loss.

### Methodology
- **Data Preprocessing**: Checked for duplicates and nulls. Selected features: `f0`, `f1`, `f2`, and `product`.
- **Modeling**: Trained a linear regression model for each region, splitting data into training and validation sets (75:25) and standardizing features. Evaluated performance with RMSE and R².
- **Profit Calculation**: Established the minimum production volume to avoid losses and calculated potential profits for the top 200 wells in each region.
- **Risk Analysis**: Used bootstrapping to estimate loss risk and profit distribution.

### Conclusions
- All datasets were clean and ready for analysis.
- The Region 2 model performed best (lowest RMSE, highest R²).
- Although Region 1 showed the highest potential profits, Region 2 is the best option due to its low risk (1.5%) and average profit of $4.5 million.