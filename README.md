# Redes neuronales
- [Red neuronal simple](https://github.com/Berishten/Redes-neuronales/blob/main/Red_neuronal_simple.ipynb)
   Implementación básica de un modelo de regresión lineal, para aproximar a un valor único utilizando reglas básicas
   de cálculo diferencial, como: derivadas, derivadas parciales.
  
   A groso modo, el modelo funciona de la siguiente manera:
     1. Predicción: la predicción del modelo se define como:
        
        $$\hat{y} = w \cdot x + b$$
     2. Cálculo de gradientes: las gradientes del MSE respecto a los parámetros 𝑤 y 𝑏 son:
        
        $$\frac{\partial \text{MSE}}{\partial w} = 2 \cdot (\hat{y} - y) \cdot x\$$
        
        $$\frac{\partial \text{MSE}}{\partial b} = 2 \cdot (\hat{y} - y)$$
        
     3. Actualización de Parámetros: los parámetros se actualizan en cada iteración usando el descenso de
        gradiente con una tasa de aprendizaje $\alpha$ hasta que el modelo converja en un valor aproximado deseado.

        $$w \leftarrow w - \alpha \cdot \frac{\partial \text{MSE}}{\partial w}$$

        $$b \leftarrow b - \alpha \cdot \frac{\partial \text{MSE}}{\partial b}$$
        
- [RN + ReLU](https://github.com/Berishten/Redes-neuronales/blob/main/RN_%2B_ReLU.ipynb)
   Esta red es muy similar a la anterior pero solo sirve para predecir un valor real positivo, además,
   se incluye el uso de:
   - Función de activación ReLU
