# Análisis y Predicción de Tráfico Aéreo

## Descripción
Este proyecto analiza y predice el tráfico aéreo de pasajeros utilizando técnicas avanzadas de ciencia de datos y aprendizaje automático. El análisis incluye:

### Análisis Temporal
- Series temporales de tráfico de pasajeros (2015-actualidad)
- Descomposición por temporadas (Invierno, Primavera, Verano, Otoño)
- Análisis de tendencias mensuales y estacionales

### Modelos Implementados
1. **Regresión Lineal Simple**
   - Variables: Mes_Numero, Mes
   - Métrica: R² Score y RMSE
   
2. **Random Forest Regressor**
   - Parámetros: n_estimators=100, max_depth=10
   - Features principales:
     - Mes_Numero
     - Temporada
     - Indicador de temporada alta
     - Pasajeros del mes anterior
   - Normalización: StandardScaler

### Predicciones Generadas
- Pronóstico a 3 meses por aeropuerto
- Predicciones por temporada (8 temporadas futuras)
- Análisis de los top 10 aeropuertos por volumen

## Dataset
El conjunto de datos (`BD_Trafico_aereo.csv`) contiene información sobre:
- Año y mes de los vuelos
- Aeropuertos de origen y destino
- Número de pasajeros
- Tipo de operación (salidas/llegadas)
- Carga y correo
- Distancias de vuelo
- Información sobre operadores aéreos

## Tecnologías Utilizadas
- **Python 3.x**
- **Bibliotecas principales:**
  - pandas: Manipulación y análisis de datos
  - numpy: Operaciones numéricas
  - scikit-learn: Modelos de machine learning
  - matplotlib/seaborn: Visualización de datos

## Metodología

### 1. Preparación de Datos
- Filtrado de vuelos de salida desde 2015
- Limpieza de datos nulos y duplicados
- Creación de características temporales
- Normalización de datos

### 2. Análisis Exploratorio
- Análisis de tendencias temporales
- Patrones estacionales por temporada
- Identificación de rutas principales
- Visualización de distribuciones de pasajeros

### 3. Modelado Predictivo
- Random Forest Regressor como modelo principal
- Validación cruzada para evaluación
- Análisis de importancia de características
- Predicciones por origen y temporada

## Ejecución

1. **Configuración del Entorno**
   ```bash
   pip install pandas numpy scikit-learn matplotlib seaborn
   ```

2. **Estructura del Proyecto**
   ```
   Proyecto 1/
   ├── BD_Trafico_aereo.csv
   ├── Trafico_aereo.ipynb
   └── README.md
   ```

3. **Uso del Notebook**
   - Abrir `Trafico_aereo.ipynb` en Jupyter Notebook o VSCode
   - Ejecutar las celdas en orden secuencial
   - Las visualizaciones se generarán automáticamente
   - Los resultados de predicción se mostrarán al final

4. **Resultados Principales**
   - Tendencias de tráfico aéreo
   - Predicciones para los próximos 3 meses
   - Análisis por temporada y origen
   - Visualizaciones interactivas

## Notas Adicionales
- El modelo está optimizado para predicciones a corto plazo
- Se recomienda actualizar el dataset periódicamente
- Los parámetros del modelo pueden ajustarse según necesidades específicas

## Contribuciones
Se aceptan contribuciones mediante Pull Requests. Para cambios mayores, por favor abrir un Issue primero para discutir los cambios propuestos.
