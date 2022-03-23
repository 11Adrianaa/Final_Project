<img src="https://bit.ly/2VnXWr2" alt="Ironhack Logo" width="100"/>

# Mejorando la predicción de un Brand Manager
*[Adriana]*

*[Ironhack Barcelona, Data Part Time]*

## Content
- [Project Description](#project-description)
- [Hypotheses / Questions](#hypotheses-questions)
- [Dataset](#dataset)
- [Analysis](#analysis)
- [Model Training and Evaluation](#model-training-and-evaluation)
- [Conclusion](#conclusion)
- [Future Work](#future-work)
- [Links](#links)

## Project Description
Con este proyecto se busca optimizar la predicción de ventas que una marca va a desarrollar a lo largo del tiempo, añadiendo además el impacto de distintas variables a través del analisis de time series.

## Hypotheses / Questions
* ¿Podemos mejorar la predicción de ventas de un brand manager?

## Dataset
* El dataset consiste en las ventas de un producto (barrera de cama) en el mercado aleman desde el día 30-09-2019 hasta el 15-03-2022.
* Para el posterior desarrollo del modelo con otras variables, se ha contado con un dataset con las mismas ventas, así como el gasto en marketing y algunas variables que también se testearon. 

## Analysis
* Pude ver que la variable de inversión en marketing era necesaria ya que podía acompañar a mi modelo inicial. Hice un estudio de su correlación y obtuve un valor interesante que me hizo seguir en la misma linea de incluirla en mi modelo. 

## Model Training and Evaluation
* Entrené dos modelos. En primer lugar un modelo SARIMAX, el cual segun los test de tendencia y de estacionalidad, no mostraba ninguna de ambas. En cambio, cuando entrené mi modelo de Neural Prophet este detectava una seasonality que lo hacia adaptarse mejor a los datos. 
* Seguí con ambos modelos, buscando los parámetros para cada uno de ellos que se adaptaran mejor a mis datos y vi que mi modelo de Neural Prophet mostraba un error inferior, así como detectaba estacionalidades que SARIMAX no. 
* Por último, seguí con el modelo de NeuralProphet para añadir la variable exogena **gasto en marketing**. Entrené y adapte los parámetros para un mejor fitting y pude obtener un modelo con capacidad predictiva. 

## Conclusion
* He podido generar un modelo que ayudará a un brand manager a conocer el comportamiento de sus ventas a futuro. 
* He visto que este modelo puede alimentarse de otras variables, dando así una visión más exacta de como las ventas van a fluctuar en el futuro con estos pará

## Future Work
Me gustaría poder añadir otras variables a mi modelo y seguir entrenandolo, con nuevos productos y otros mercados. De esta forma permitiría a los brand managers contar con una herramienta mucho más exacta que las posibles predicciones que puedan obtener de ventas pasadas.


## Links

[Repository](https://github.com/11Adrianaa/Final_Project)  