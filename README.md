# 📊 Predicción de Churn y Estrategias de Retención de Clientes

## Descripción del Proyecto

Este proyecto tiene como objetivo **identificar clientes con riesgo de cancelación (churn)** utilizando técnicas de **Machine Learning**, y **proponer estrategias de retención** basadas en los factores más determinantes que afectan la fidelización de los clientes.

Se utiliza un **Modelo Champion** entrenado sobre datos históricos, que permite predecir:

- La **probabilidad de churn** para cada cliente.
- La **etiqueta de cancelación** (`Churn = 0/1`).

El proyecto forma parte del curso anual de **Ciencia de Datos de Alura Latam**, auspiciado por **Oracle**, y fue desarrollado por **Leandro Puebla Martínez**.  

---

## Estructura del Repositorio


├── data/
│   └── datos_originales.csv      # Dataset original de clientes
├── notebooks/
│   └── analisis_churn.ipynb     # Notebook con predicciones, análisis y visualizaciones
├── modelo_champion.pkl           # Modelo Champion entrenado
├── predicciones_churn.xlsx       # Predicciones generadas por el modelo
├── predicciones_churn.csv        # Predicciones en CSV para análisis externo
├── README.md                     # Documentación del proyecto


---

## Funcionalidades Principales

1. **Carga y preparación del Modelo Champion**  
   - Se asegura que las columnas del dataset coincidan con las del modelo entrenado.
   - Carga el modelo desde archivo `.pkl` o `.joblib`.

2. **Generación de Predicciones de Churn**  
   - Devuelve un DataFrame con:
     - `ID_cliente`
     - `Probabilidad_Churn`
     - `Churn` (0/1)

3. **Exportación de Resultados**  
   - Guarda las predicciones en **Excel** (`predicciones_churn.xlsx`) para análisis y seguimiento posterior.

4. **Análisis de Clientes de Mayor Riesgo**  
   - Identifica los 10 clientes con mayor probabilidad de churn.
   - Genera visualizaciones gráficas para facilitar la interpretación de resultados.

5. **Informe de Factores Clave y Estrategias de Retención**  
   - Evalúa variables más relevantes que influyen en la cancelación.
   - Proporciona recomendaciones estratégicas para fidelización y retención de clientes.

---

## Flujo del Proyecto

1. **Preparación de Datos**  
   - Limpieza y codificación de variables categóricas.
   - Adaptación de columnas al formato esperado por el modelo Champion.

2. **Carga del Modelo y Predicciones**  
   - Carga del modelo entrenado (`modelo_champion.pkl`).
   - Predicción de probabilidades de churn y etiquetas de cancelación.

3. **Análisis y Visualización**  
   - Identificación de clientes con mayor riesgo.
   - Generación de gráficos para análisis exploratorio.

4. **Exportación de Resultados**  
   - Guardado del DataFrame final con predicciones a Excel.
   - Descarga lista para revisión o uso en campañas de retención.

5. **Informe y Estrategias de Retención**  
   - Documentación de factores clave.
   - Propuestas de acción para aumentar la fidelización.

---

## Factores Clave que Impactan la Cancelación

- **Cantidad de servicios contratados**: Menor número de servicios incrementa el riesgo de churn.  
- **Tiempo de relación con la empresa**: Clientes recientes presentan mayor probabilidad de abandono.  
- **Actividad e interacciones recientes**: Baja frecuencia de uso reduce engagement.  
- **Historial de incidencias**: Retrasos en pagos o reclamos frecuentes elevan el riesgo.  
- **Adopción de canales digitales**: Clientes con baja utilización de apps o plataformas online muestran mayor tendencia a cancelar.

---

## Resultados y Conclusiones

El **Modelo Champion** permite identificar clientes en riesgo con buena precisión. Aplicando estrategias focalizadas y personalizadas basadas en los factores identificados, se pueden lograr beneficios como:

- Reducción de la cancelación de clientes.
- Mejora del engagement y la fidelización.
- Maximización de la satisfacción del cliente y del valor a largo plazo.

---

## Recomendaciones Estratégicas

- **Programas de fidelización**: Ofrecer beneficios, descuentos o promociones personalizadas.  
- **Upselling y cross-selling**: Incrementar la contratación de servicios complementarios.  
- **Seguimiento proactivo**: Monitorear clientes con baja actividad o incidencias frecuentes.  
- **Comunicación personalizada**: Campañas segmentadas según el perfil de riesgo.  
- **Optimización de canales digitales**: Incentivar la adopción de apps y plataformas online.

---

## Tecnologías Utilizadas

- **Python 3.12**  
- **Pandas, NumPy** – Manipulación de datos  
- **Scikit-Learn** – Modelado de Machine Learning  
- **Seaborn, Matplotlib** – Visualización de datos  
- **Jupyter Notebook** – Desarrollo interactivo  
- **OpenPyXL** – Exportación de resultados a Excel

---

## Créditos

Desarrollado por: **Leandro Puebla Martínez**  
Curso: **Ciencia de Datos**, **Alura Latam**  
Auspiciado por: **Oracle**

---

## Contacto

- GitHub: [https://github.com/Leanga87](https://github.com/Leanga87)  
- Email: lean.gapm@gamail.com
