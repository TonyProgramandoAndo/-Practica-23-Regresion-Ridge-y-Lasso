Práctica #23: Regresión Ridge y Lasso

🔹 Paso 1: Configuración Inicial
✅ Carga el set de datos que puedes encontrar en el campus virtual ✅ Ejecutar las celdas de importación de librerías y carga del dataset.
✅ Familiarizarse con los datos usando .head(), .info() y .describe().

🔹 Paso 2: Análisis Exploratorio (EDA)
📊 Para variables numéricas:

Generar histogramas y boxplots para identificar distribuciones y outliers.
Calcular medidas de tendencia central y dispersión.
📊 Para variables categóricas:

Usar gráficos de barras para visualizar frecuencias.
🔹 Paso 3: Matriz de Correlación
✅ Calcular la matriz de correlación solo para variables numéricas.
✅ Generar un mapa de calor para visualizar relaciones.
📌 Pregunta: ¿Qué variables están más correlacionadas con el target (charges)? (salida del dataset)

🔹 Paso 4: Preprocesamiento
🔧 Tareas:

Manejar valores faltantes con SimpleImputer.
Codificar variables categóricas con OneHotEncoder.
Estandarizar variables numéricas con StandardScaler.
✅ Verificar que el dataset transformado no tenga valores nulos.
🔹 Paso 5: Modelado (Lasso y Ridge)
🎯 Para cada modelo:

Ajustar el modelo con los hiperparámetros dados (alpha=0.1 para Lasso, alpha=1.0 para Ridge).
Calcular MSE y R² para evaluar rendimiento.
Analizar los coeficientes para identificar variables importantes.
📌 Pregunta:

¿Qué modelo tiene un mejor R²? ¿Por qué crees que ocurre esto?
¿Qué variables tienen coeficientes cercanos a cero en Lasso? ¿Por qué?
🔹 Paso 6: Verificación de Supuestos
📉 Para cada modelo, verificar:

Linealidad (gráfico de residuos vs predicciones).
Normalidad de residuos (QQ-Plot y test de Shapiro-Wilk).
Homocedasticidad
Multicolinealidad (VIF > 10 indica problema).
📌 Pregunta:

¿Se cumplen los supuestos en ambos modelos?
Si hay heterocedasticidad, ¿cómo podría solucionarse?
🔹 Paso 7: Comparación Final
📊 Analizar:

¿Qué modelo es más interpretable?
¿Cuál reduce mejor el sobreajuste?
¿Qué variables son más importantes en cada caso?
