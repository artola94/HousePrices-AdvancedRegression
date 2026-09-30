# House Prices - Advanced Regression Techniques

Predicción del precio de venta para la [competición de Kaggle](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques). La métrica es el RMSLE.

**Score: 0.11515** en el leaderboard público, con TabPFN v2. **Resultado TOP 1%**

El cuaderno es `nb_HousePrices.ipynb`.

La solución es **TabPFN v2**, sin ninguna mezcla o voting. Se entrena en cinco particiones, con semilla 42 y sin early stopping. La variable objetivo está en log1p. Cada partición predice el test y el envío es la media de esas cinco predicciones. Además de eso, las categóricas entran como texto. El train supera el límite por defecto del modelo, así que ese límite se ignora.