# Análisis de Modelos Lineales y Algoritmos de Optimización en Datos de Propiedades
#### Fecha: Noviembre 28, 2024

---
Este repositorio contiene el trabajo final del curso de Introducción a los Problemas Básicos de Administración y Economía, donde analizamos la relación entre la superficie cubierta y el precio de venta de propiedades en el barrio de Boedo, Ciudad de Buenos Aires. Utilizamos modelos lineales y algoritmos de optimización para ajustar los datos y evaluar su efectividad.

## Tabla de Contenidos  
1. [Introducción](#introducción)  
2. [Metodología](#metodología)  
3. [Resultados](#resultados)  
4. [Conclusiones](#conclusiones)  
5. [Estructura del Repositorio](#estructura-del-repositorio)  
6. [Autores](#autores)  
7. [Licencia](#licencia)  

---

## Introducción  
El objetivo de este proyecto es explorar el uso de métodos de optimización y modelos lineales para predecir el precio de venta de propiedades. Trabajamos con datos reales provistos por Properati y comparamos la efectividad de diferentes técnicas de ajuste, como Luus-Jaakola, gradiente descendente y mínimos cuadrados ordinarios (lm).  

---

## Metodología  
1. **Modelo Propuesto**:  
   Utilizamos un modelo lineal simple para estimar el precio basado en la superficie cubierta:  

   \[
   \hat{Precio} = \mu + \alpha \cdot Sup
   \]

2. **Evaluación del Modelo**:  
   Empleamos el error cuadrático medio (MSE) para medir el ajuste del modelo. También se exploraron otras métricas como el error absoluto medio (MAE).  

3. **Optimización**:  
   - Luus-Jaakola: Algoritmo estocástico de optimización.  
   - Gradiente Descendente: Algoritmo iterativo basado en el gradiente de la función de pérdida.  
   - Mínimos Cuadrados Ordinarios (lm): Solución analítica como referencia.  

---

## Resultados  
- Los tres métodos convergieron a soluciones similares, demostrando la efectividad de las técnicas de optimización para funciones convexas.  
- Se observó que la superficie cubierta tiene una relación positiva con el precio de venta.  

| Método                | Mu         | Alpha     | MSE          |  
|-----------------------|------------|-----------|--------------|  
| Luus-Jaakola          | 137,722.9  | 1,159.35  | 8,740,642,890|  
| Gradiente Descendente | 109,601.8  | 1,254.23  | 8,593,462,003|  
| lm()                  | 109,601.8  | 1,254.23  | 8,593,462,003|  

---

## Conclusiones  
- Los algoritmos implementados son efectivos y producen resultados consistentes con los métodos analíticos.  
- Se recomienda incluir más variables para mejorar el modelo, como fondo, cantidad de habitaciones y características del barrio.  

---

### Autores:
- Lorenzo Marquesini
- Agustín Orue
- Juan Cruz Chierasco
- Marco Di Sario

---


## Licencia  
Este proyecto se distribuye bajo la Licencia MIT.  

--- 