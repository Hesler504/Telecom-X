🧠 Sección 1: Configuración inicial

    Importación de librerías: pandas, matplotlib.pyplot, numpy, datetime, seaborn.

    Configuración del estilo gráfico.

    Lectura de datos desde 'datasets/demand.csv'.

    Conversión de columna date a datetime y establecimiento como índice.

📊 Sección 2: Visualización de series de tiempo

    Se grafica la serie de demanda original con plt.plot().

    Se realiza un gráfico de descomposición de la serie (tendencia, estacionalidad, ruido) usando seasonal_decompose.

🧪 Sección 3: Prueba de estacionariedad

    Prueba de Dickey-Fuller aumentada (adfuller) para determinar si la serie es estacionaria.

    Si no es estacionaria, se realiza diferenciación y se vuelve a aplicar la prueba.

🔢 Sección 4: Modelado ARIMA

    Uso de auto_arima para seleccionar los mejores parámetros (p, d, q) automáticamente.

    Ajuste del modelo ARIMA.

    Pronóstico a futuro (30 días).

    Gráfico con valores reales y predicciones.

🏭 Sección 5: Modelado con Prophet

    Preparación de datos en el formato requerido por Prophet (ds, y).

    Entrenamiento del modelo Prophet.

    Predicción a futuro (90 días).

    Visualización del pronóstico y sus componentes (tendencia, estacionalidad).

🤖 Sección 6: Modelado con LSTM (Red Neuronal)

    Escalado de datos con MinMaxScaler.

    División de datos en entrenamiento y prueba.

    Construcción de un modelo secuencial LSTM con Keras:

        Capas: LSTM, Dense.

        Compilación con adam y mean_squared_error.

    Entrenamiento del modelo.

    Predicción y visualización.

📈 Sección 7: Comparación de modelos

    Cálculo del Error Cuadrático Medio (RMSE) para:

        ARIMA

        Prophet

        LSTM

    Visualización comparativa de las predicciones de los tres modelos.

✅ Estado general del notebook

    Todo el código está bien estructurado.

    Se utilizan prácticas estándar de análisis de series de tiempo.

    Los modelos están correctamente implementados y comparados.
