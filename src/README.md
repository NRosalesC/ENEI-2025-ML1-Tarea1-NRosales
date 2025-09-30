### Deliverables
You must fork the [original repository](), and turn in a link to your groups repository with:

* A Jupyter notebook (in the `src` folder) with:

  * Your `numpy` implementations for OLS and gradient descent,
  * Plots: cost-function convergence, coefficient paths, predicted vs. actual values.
* A write-up in Markdown. Replace the contents of this file (`README.md`) with:
  
  * The names of your group's members,
  * Differences observed between OLS, Ridge, and Lasso,
  * Effect of learning rate on gradient descent,
  * How k-fold cross-validation influenced the choice of regularization strength.

# Entrega Tarea 1 - ML1

## Integrantes del grupo
- Noel Rosales Chuco
- [Nombre 2]
- [Nombre 3]

---

## Diferencias observadas entre OLS, Ridge y Lasso

- **OLS (Mínimos Cuadrados Ordinarios):** Ajusta todos los coeficientes sin penalización. Puede sobreajustar si hay muchas variables o colinealidad.  
- **Ridge:** Penaliza la magnitud de los coeficientes (L2). Reduce el overfitting manteniendo todos los coeficientes distintos de cero.  
- **Lasso:** Penaliza la suma de los valores absolutos de los coeficientes (L1). Puede forzar algunos coeficientes a cero, realizando selección automática de variables.

---

## Efecto de la tasa de aprendizaje en el descenso de gradiente

- Una **tasa de aprendizaje muy alta** puede provocar que el algoritmo no converja o que oscile alrededor del mínimo.  
- Una **tasa de aprendizaje muy baja** hace que la convergencia sea muy lenta.  
- Ajustando adecuadamente la tasa de aprendizaje, el descenso de gradiente logra aproximarse al mínimo de la función de costo de manera eficiente.

---

## Influencia de la validación cruzada k-fold en la elección de la fuerza de regularización

- Se utilizó **validación cruzada de 5 pliegues (5-fold CV)** para probar diferentes valores de alpha en Ridge y Lasso.  
- La **media del R² o del MSE** en los pliegues permitió seleccionar el alpha que mejor generaliza a datos no vistos.  
- Esto evita escoger un valor de alpha basado solo en el conjunto de entrenamiento, mejorando la robustez del modelo.

---
