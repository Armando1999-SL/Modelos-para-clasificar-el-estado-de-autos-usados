# Modelos para clasificar el estado de autos usados (Clasificación Ordinal vs. Métodos Clásicos de ML)

Este proyecto tiene como objetivo **comparar modelos de Machine Learning diseñados para datos ordinales** frente a sus versiones clásicas que no consideran este tipo de estructura.

## Descripción del problema

El caso de estudio consiste en la **clasificación del estado de autos usados** en función de características ordinales relacionadas con el automóvil.  

Las variables consideradas son:  
- Precio de compra  
- Precio de mantenimiento  
- Número de puertas  
- Capacidad de personas  
- Tamaño del maletero  
- Nivel de seguridad estimado  

Con base en estas características, los automóviles se clasifican en las siguientes categorías:  
- Muy bueno  
- Bueno  
- Aceptable  
- Inaceptable  

## Enfoque de solución

Se evaluaron distintos algoritmos en sus versiones **clásicas** y **adaptadas a la ordinalidad** de los datos:  

- **Regresión logística** → Modelo de probabilidades proporcionales y modelo proporcional de hazard  
- **Adaboost** → Boosting de división fija  
- **Redes neuronales** → Redes neuronales ordinales  
- **Árboles de decisión** → Árboles de decisión ordinal  
- **Random Forest** → Random Forest ordinal  

### Métricas de evaluación

Para comparar el desempeño de los modelos se emplearon:  
- **Mean Absolute Error (MAE)**  
- **Kappa de Cohen (ordinal)**  

## Resultados

Los resultados muestran que los **modelos que consideran la ordinalidad de los datos** tienden a obtener un mejor desempeño en comparación con sus contrapartes clásicas.  

En este caso, el **Random Forest ordinal** fue el modelo que alcanzó las mejores métricas de evaluación, con un **MAE = 0.3** y **Kappa = 0.95**.
