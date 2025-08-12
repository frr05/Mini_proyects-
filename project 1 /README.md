# ✈️ Predicción de Demanda Aérea Mensual en Chile

## 📌 Descripción
Este proyecto tiene como objetivo predecir la cantidad mensual de pasajeros transportados en vuelos nacionales e internacionales en Chile. Se utiliza un modelo de **regresión lineal** entrenado con datos históricos provenientes del portal **Datos Abiertos del Gobierno de Chile**.

El enfoque es demostrar habilidades clave de **Data Engineering**:
- Extracción y limpieza de datos públicos.
- Ingeniería de variables (features) a partir de fechas.
- Entrenamiento y evaluación de modelos predictivos.
- Visualización y comunicación de resultados.

## 📊 Dataset
- **Fuente:** [Datos Abiertos Chile - Tráfico Aéreo](https://datos.gob.cl/dataset/trafico-aereo-en-aeropuertos-chilenos)
- **Variables principales:**
  - `Mes`
  - `Año`
  - `Pasajeros_nacionales`
  - `Pasajeros_internacionales`
  - `Total_pasajeros`

## 🛠 Tecnologías usadas
- Python 3
- pandas
- matplotlib / seaborn
- scikit-learn
- Jupyter Notebook

## 📈 Metodología
1. **Carga y limpieza** del dataset.
2. **Ingeniería de variables**:
   - Conversión de fechas.
   - Creación de variable "temporada alta/baja".
3. **Entrenamiento** de un modelo de regresión lineal.
4. **Evaluación** con métricas MSE y R².
5. **Visualización** de valores reales vs. predicciones.

## 🚀 Ejecución
1. Clonar el repositorio.
2. Instalar dependencias:
   ```bash
   pip install pandas matplotlib seaborn scikit-learn jupyter

