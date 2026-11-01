# Analisis Exploratorio de Datos (EDA): Salarios en Ciencia de Datos

@ Proyecto Final - Fundamentos de Ciencia de Datos (Ucamp / UTEL)
@ Desarrollado por: Ramon Ceja Cervantes (Ray)
@ Licenciatura: Ingenieria Computacional

---

## 1. Descripcion del Proyecto

Este repositorio contiene el desarrollo y documentacion del analisis exploratorio de datos (EDA) enfocado en el mercado global de salarios dentro de la industria de ciencia de datos (2020 - 2022), utilizando la base de datos oficial de Kaggle.

El objetivo principal consistio en evaluar las distribuciones salariales en USD, analizar la adopcion del trabajo remoto, examinar correlaciones entre variables cuantitativas y generar visualizaciones interactivas mediante el ecosistema de Plotly y Pandas.

---

## 2. Preparacion del Entorno y Requisitos

@ Sistema operativo: Linux (CachyOS) / Shell: Fish
@ Editor: Visual Studio Code + Jupyter Extension
@ Entorno virtual: `.venv`

Para ejecutar la libreta de manera local y asegurar la compatibilidad de paquetes, se incluye el archivo `requirements.txt`.

1. Clonar el repositorio:
```fish
git clone https://github.com/ramon-ceja/ucamp-kaggle-datasets.git
cd tu-repositorio
```

2. Activar el entorno virtual:
```fish
source .venv/bin/activate.fish
```

3. Instalar dependencias requeridas:
```fish
pip install -r requirements.txt
```

---

## 3. Hallazgos Clave del Analisis (Insights)

# Tendencia Temporal Incrementativa: Entre 2020 y 2022 se observa una clara tendencia al alza en la media salarial bruta estandarizada en USD, reflejando una demanda creciente de talento especializado tras la consolidacion del sector post-pandemia.

# Prevalencia del Trabajo Remoto: La distribucion del `remote_ratio` evidencia que mas del 70% de la muestra opera bajo modalidades totalmente remotas (100%) o hibridas (50%), demostrando la alta flexibilidad geografica de la industria.

# Factores Determinantes de Compensacion: El analisis de correlacion de Pearson muestra coeficientes cercanos a cero entre variables cuantitativas puras (como año o ratio remoto frente al salario), confirmando que las variaciones salariales mas significativas (outliers superiores a $300k USD) estan condicionadas por variables cualitativas como el nivel de experiencia (`SE`/`EX`) y el pais de la sede corporativa (`company_location`).

# Asimetria en la Densidad Salarial: La estimacion de densidad de Kernel (KDE) y los histogramas confirman una distribucion con sesgo positivo (a la derecha), donde la mediana ($101,570 USD) se posiciona por debajo de la media ($112,297 USD), ubicando la mayor concentracion de profesionales en el rango de $50k a $130k USD anuales.

---

## 4. Estructura del Proyecto

# 1. Preparacion de entorno e importacion de dependencias
# 2. Diagnostico del DataFrame (Ficha tecnica y completitud)
# 3. Analisis de frecuencias y agrupaciones por categoria
# 4. Estimacion de densidad de distribucion salarial (KDE)
# 5. Matriz de correlacion lineal de Pearson
# 6. Conclusiones finales y referencias