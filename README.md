# 📊 Proyecto ConnectaTel – Análisis y Segmentación de Clientes

## 📌 Objetivo del proyecto

El objetivo de este proyecto es analizar el comportamiento de los clientes de ConnectaTel mediante técnicas de limpieza, exploración y segmentación de datos. A partir de la información de usuarios y su historial de uso, se busca identificar patrones de consumo, detectar problemas en los datos y generar insights que permitan crear estrategias comerciales y nuevos planes adaptados a diferentes perfiles de clientes.

---

## 📁 Datasets utilizados

Se trabajó con tres conjuntos de datos:

### `plans.csv`
Contiene información de los planes disponibles para los usuarios.

Variables relevantes:
- tipo de plan
- características del plan

### `users_latam.csv`
Contiene información demográfica y administrativa de los usuarios.

Variables relevantes:
- `user_id`
- `first_name`
- `last_name`
- `age`
- `city`
- `reg_date`
- `plan`
- `churn_date`

### `usage.csv`
Contiene el historial de uso de servicios por usuario.

Variables relevantes:
- `user_id`
- `date`
- `type`
- `duration`
- `length`

---

## 🧪 Etapas del análisis realizadas

### 1. Carga y exploración inicial
- Importación de librerías
- Carga de datasets
- Exploración con `.head()`, `.shape()` y `.info()`

### 2. Identificación de problemas de calidad
- Detección de valores nulos
- Identificación de sentinels
- Revisión de columnas numéricas y categóricas
- Validación de fechas

### 3. Limpieza de datos
- Reemplazo de sentinels (`-999`)
- Conversión de `"?"` a valores nulos
- Corrección de fechas fuera de rango
- Tratamiento de datos faltantes

### 4. Creación de métricas por usuario
Se construyeron variables agregadas:

- cantidad total de mensajes
- cantidad total de llamadas
- minutos totales de llamadas

Posteriormente se integraron con la tabla de usuarios.

### 5. Análisis exploratorio y visualización
Se generaron:

- histogramas
- boxplots
- análisis de distribución
- detección de outliers

Variables analizadas:

- edad
- mensajes
- llamadas
- minutos

### 6. Segmentación de clientes
Se crearon segmentos según:

**Nivel de uso**
- Bajo uso
- Uso medio
- Alto uso

**Grupo por edad**

Y se analizaron patrones por plan y comportamiento.

### 7. Generación de insights ejecutivos
Se desarrollaron recomendaciones enfocadas en:

- optimización de planes
- identificación de clientes valiosos
- oportunidades comerciales

---

## ▶️ Cómo ejecutar el proyecto

### Opción 1: Google Colab

1. Descarga el archivo `.ipynb`
2. Abre Google Colab
3. Selecciona:

Archivo → Subir notebook

4. Sube el notebook
5. Carga los datasets en la carpeta correspondiente
6. Ejecuta las celdas en orden

---
## 🔁 Guía de reproducción

1. Clona el repositorio:

```bash
git clone URL_DEL_REPOSITORIO
```

2. Instala las librerías:

```bash
pip install pandas numpy matplotlib seaborn
```

3. Verifica que estén los archivos:

```text
plans.csv
users_latam.csv
usage.csv
```

4. Abre el notebook en Google Colab, Jupyter o VS Code.

5. Ejecuta las celdas en orden.

Al finalizar podrás visualizar limpieza de datos, análisis, segmentación e insights.
