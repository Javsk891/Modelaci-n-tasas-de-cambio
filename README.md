# Modelaci-n-tasas-de-cambio
Este código se centra en la implementación del modelo GARCH y otros modelos de ML para pronosticar la volatilidad del dólar canadiense en relación con el dólar estadounidense.

# **Fase 1: Modelación del retorno de la tasa de cambio USD/CAD mediante modelos de la familia GARCH**

Este código se centra en la implementación del modelo GARCH para pronosticar la volatilidad del dólar canadiense en relación con el dólar estadounidense. El enfoque GARCH permite capturar la naturaleza dinámica de la volatilidad, considerando la autocorrelación y la heterocedasticidad condicional de los rendimientos del tipo de cambio.

A través de este código, exploraremos cómo utilizar el método GARCH para analizar y anticipar la volatilidad del par de divisas USD/CAD, brindando así información valiosa para la toma de decisiones en los mercados financieros.

# **Fase 2: Predicción del precio de la tasa de cambio seleccionada mediante modelos de redes neuronales.**

Los modelos de redes neuronales han revolucionado la forma en que abordamos problemas complejos en diversos campos, incluida la predicción financiera. En el contexto de los mercados de divisas, donde la volatilidad juega un papel crucial en la toma de decisiones de inversión, las redes neuronales ofrecen un enfoque prometedor para modelar y predecir la volatilidad del tipo de cambio entre el dólar canadiense (CAD) y el dólar estadounidense (USD).

A continuación exploraremos cómo los modelos de redes neuronales pueden ser aplicados para calcular y predecir la volatilidad del CAD respecto al USD, ofreciendo una perspectiva innovadora y potencialmente valiosa para los inversores y operadores en el mercado de divisas.

**Predicción con redes neuronales recurrentes RNN**

Las redes neuronales recurrentes (RNN) ofrecen un enfoque poderoso para modelar y predecir la volatilidad del tipo de cambio entre el dólar canadiense (CAD) y el dólar estadounidense (USD).

Las RNN son capaces de capturar patrones complejos en datos secuenciales, lo que las convierte en una herramienta adecuada para analizar series temporales de precios de divisas y otras variables relevantes. Al utilizar datos históricos de precios, indicadores técnicos y factores macroeconómicos, las RNN pueden aprender y extrapolar las relaciones subyacentes en los datos para predecir la volatilidad futura del CAD respecto al USD.

*   El modelo de RNN tiene un buen rendimiento en el conjunto de entrenamiento, con un RMSE de 0.006766965566283014. Esto significa que el modelo es capaz de predecir con precisión los valores de la serie de tiempo en el conjunto de entrenamiento.
*   El modelo de RNN tiene un rendimiento ligeramente mejor en el conjunto de validación, con un RMSE de 0.005384960213896202. Esto significa que el modelo es capaz de generalizar bien a datos nuevos que no se utilizaron para entrenar el modelo.
*   El modelo de RNN tiene el mejor rendimiento en el conjunto de prueba, con un RMSE de 0.004748733718178748. Esto significa que el modelo es capaz de predecir con precisión los valores de la serie de tiempo en datos que no se utilizaron ni para entrenar ni para validar el modelo.

# **Prediccion con redes neuronales FeedForward**

Los modelos feedforward son una clase popular de redes neuronales artificiales que constan de múltiples capas, incluyendo capas de entrada, capas ocultas y capas de salida. Estos modelos son capaces de aprender relaciones complejas entre los datos de entrada y las etiquetas de salida, lo que los hace adecuados para modelar y pronosticar la volatilidad en los mercados financieros.

A continuación exploraremos cómo implementar modelos feedforward para la predicción de la volatilidad del par de divisas CAD/USD. Utilizando datos históricos de precios, indicadores técnicos y otros factores relevantes, estos modelos pueden ofrecer predicciones precisas y oportunas de la volatilidad, proporcionando así una herramienta valiosa para los inversores y operadores en el mercado de divisas.

*   El modelo Feedforward ha obtenido un buen rendimiento en la predicción de la volatilidad del CAD respecto al USD. Esto se puede observar en los valores de RMSE relativamente bajos para los tres conjuntos de datos.
*   El modelo Feedforward ha obtenido el mejor rendimiento en el conjunto de prueba. Esto significa que el modelo es capaz de generalizar bien a datos nuevos que no fueron utilizados para entrenarlo.
*   El modelo Feedforward ha obtenido un rendimiento ligeramente mejor que el modelo RNN. Esto se puede observar en la comparación de los valores de RMSE para los dos modelos.

**Predicción con Naive Bayes**

El modelo Naive Bayes es un clasificador probabilístico simple pero efectivo que se basa en el teorema de Bayes y asume independencia condicional entre las características. Aunque su simplicidad puede parecer una limitación, el modelo Naive Bayes ha demostrado su utilidad en una variedad de aplicaciones, incluido el análisis financiero.

A continuación exploraremos cómo el modelo Naive Bayes puede ser utilizado para calcular la volatilidad del CAD respecto al USD. Al aprovechar datos históricos, indicadores financieros y otros factores relevantes, el modelo Naive Bayes puede proporcionar estimaciones confiables de la volatilidad futura, ofreciendo así una perspectiva valiosa para los participantes del mercado financiero.

**Conclusiones**

*   El modelo Feedforward ha obtenido un rendimiento ligeramente mejor que el modelo RNN. Esto se puede observar en la comparación de los valores de RMSE para los dos modelos, sin embargo al comparar los valores de MSE, MAE y MAPE para los cuatro modelos, podemos identificar el modelo con el mejor rendimiento general. En este caso, el Modelo RNN presenta los valores más bajos para las tres métricas:

MSE: 0.000037

MAE: 0.004583

MAPE: 0.347789

Esto sugiere que el Modelo RNN tiene el mejor ajuste a los datos y produce predicciones más precisas en comparación con los otros tres modelos.

*   Ambos modelos, RNN y Feedforward, han obtenido un buen rendimiento en la predicción de la volatilidad del CAD respecto al USD. Esto se puede observar en los valores de RMSE relativamente bajos para los tres conjuntos de datos.

*   El modelo RNN ha obtenido un mejor rendimiento en el conjunto de entrenamiento que el model FeedForward. Esto significa que el modelo RNN se ajusta mejor a los datos de entrenamiento que el modelo Feedforward.

*   Los modelos de redes neuronales muestran un mejor rendimiento que Naive Bayes, lo que nos muestra claramente que la modelación ayuda a obtener mejores predicciones para la volatilidad
