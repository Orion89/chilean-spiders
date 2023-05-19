# Identificando arácnidos chilenos a través de *deep metric learning*

![embeddings_animation](https://github.com/Orion89/chilean-spiders/blob/main/animations/anim_embs_model_2-b-hard-squared-dist_50cls_29ep_080323.gif)

Proyecto para identificar arácnidos que habitan el territorio de Chile a través de determinar un vector a partir de una fotografía del animal, la cual es procesada a través de una red *ResNet50* que actúa como *features extractor*. Una vez obtenido el vector correspondiente a la fotografía, se busca el vector más cercano entre los datos de entrenamiento calculando la distancia euclideana al cuadrado entre el *embedding* de consulta y los vectores de ajuste, asignando a la fotografía la clase del vecino (vector) más cercano.

Se puede acceder al servicio en el siguiente sitio: https://nearest-spiders-production.up.railway.app/

El sitio es una *app* muy sencilla desarrollada con **Dash**, la cual consume el modelo entrenado a través de una API desarrollada con **FastAPI**.

