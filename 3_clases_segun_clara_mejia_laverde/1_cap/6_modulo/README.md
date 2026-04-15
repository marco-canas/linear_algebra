# Módulo 6: Geometría de los Datos - Subespacios Fundamentales de una Matriz

[](https://www.python.org/downloads/)
[](https://opensource.org/licenses/MIT)
[](https://es.wikipedia.org/wiki/Bajo_Cauca)

## Descripción del Módulo

Este módulo aborda la teoría de los **Subespacios Asociados a una Matriz** (Espacio Nulo, Columna y Fila) aplicada a la resolución de problemas reales en la **Ingeniería Agropecuaria** y la **Administración de Empresas**.

En el contexto del **Bajo Cauca Antioqueño**, aplicamos estas técnicas para optimizar el uso de sensores en cultivos tecnificados y mejorar la eficiencia logística de la distribución de insumos en la región de Caucasia.

-----

## Objetivos de Aprendizaje

  * **Matemáticos:** Identificar bases y dimensiones de los subespacios fundamentales de una matriz $A \in \mathbb{R}^{m \times n}$.
  * **Computacionales:** Implementar algoritmos en Python (`NumPy`, `SciPy`) para calcular el rango y la nulidad.
  * **Aplicados:** Detectar redundancia en sistemas de sensores (Agricultura de Precisión) y optimizar rutas de suministro administrativo.

-----

## Situaciones Problemáticas Regionales

### 1\. Optimización de Sensores (Arroz y Ganadería)

Utilizamos el **Espacio Nulo** para identificar redundancias en redes de sensores de humedad y temperatura en cultivos del Bajo Cauca. Si la nulidad es mayor a cero, simplificamos la red para reducir costos operativos.

### 2\. Logística en Caucasia

Analizamos el **Espacio Fila** de las matrices de costos de transporte entre centros de acopio regionales para eliminar rutas linealmente dependientes, optimizando el margen de contribución de las empresas locales.

-----

## Herramientas Utilizadas

  * **Lenguajes:** Python (NumPy, Pandas, Plotly).
  * **Notación:** $\LaTeX$ para rigor matemático.
  * **Plataformas:** GitHub (Control de versiones) y YouTube (Storytelling técnico).

-----

## Estructura del Repositorio

```bash
├──  notebooks/
│   └── 06_subespacios_matriz.ipynb   # Clase interactiva y visualizaciones
├── data/
│   ├── sensores_suelo.csv           # Dataset artificial de agricultura
│   └── logistica_insumos.csv        # Dataset de administración regional
├── scripts/
│   └── subespacios_utils.py         # Funciones auxiliares para Rango y Nulidad
└── README.md                        # Documentación principal (este archivo)
```

-----

## Ejemplo de Código Rápido

```python
import numpy as np

# Definición de la matriz de sensores (Bajo Cauca)
A = np.array([[25, 60, 400],   # Temp, Hum, Rad
              [50, 120, 800]]) # Sensor redundante (2*Fila1)

# Cálculo del Rango
rango = np.linalg.matrix_rank(A)
print(f"Información independiente (Rango): {rango}")
```

-----

## Referentes

  * **Pedagogía:** Basado en la estructura de clase de la Prof. **Clara Mejía Laverde**.
  * **Matemáticas:** Gilbert Strang, *Linear Algebra and Its Applications*.
  * **Ciencia de Datos:** Ian Goodfellow, *Deep Learning*.

-----

**Contribuidor:** Marco Julio Cañas Campillo.  
**Institución:** Curso de Álgebra Lineal - Enfoque Agroindustrial  
**Contacto:** marco.canas@udea.edu.co | [Link a YouTube](https://www.youtube.com/@DiMathData) 

-----

### Instrucciones para el Estudiante:

1.  Haz un **Fork** de este repositorio.
2.  Completa los ejercicios propuestos en el archivo `notebooks/06_subespacios_matriz.ipynb`.
3.  Sube un video a **YouTube** explicando la importancia del Espacio Nulo en la reducción de costos de sensores y enlaza el video en tu entrega final.