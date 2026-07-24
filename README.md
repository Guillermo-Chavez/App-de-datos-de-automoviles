# 🚗 App de Datos de Automóviles

![Python](https://img.shields.io/badge/Python-3.9%2B-3776AB?logo=python&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?logo=streamlit&logoColor=white)
![Plotly](https://img.shields.io/badge/Plotly-3F4F75?logo=plotly&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-150458?logo=pandas&logoColor=white)
![status](https://img.shields.io/badge/status-en%20producción-brightgreen)

Aplicación web interactiva construida con **Streamlit** para explorar un conjunto de datos de anuncios de venta de vehículos en Estados Unidos (precio, año, modelo, condición, cilindros, combustible, odómetro, transmisión, tipo de vehículo, color, tracción, entre otros). Mediante gráficos dinámicos generados con **Plotly**, el usuario puede identificar patrones y tendencias que apoyan el análisis exploratorio de datos (EDA).

### 🔗 [Ver demo en vivo](https://web-site-p9yw.onrender.com)

> ⏳ La app está alojada en el plan gratuito de Render: si nadie la visitó recientemente puede tardar 30–60 segundos en "despertar" la primera vez que abras el enlace.

---

## 📑 Tabla de contenido

- [Funcionalidades](#-funcionalidades)
- [Demo](#-demo-en-vivo)
- [Dataset](#-dataset)
- [Tecnologías](#️-tecnologías)
- [Instalación y uso local](#-instalación-y-uso-local)
- [Estructura del repositorio](#-estructura-del-repositorio)
- [Próximos pasos](#-próximos-pasos)
- [Licencia](#-licencia)

---

## ✨ Funcionalidades

| Gráfico | Descripción |
|---|---|
| 📊 **Histograma del odómetro** | Distribución del kilometraje de los vehículos anunciados |
| 📈 **Precio vs. odómetro** | Gráfico de dispersión para analizar la relación entre ambas variables |
| 📊 **Tipos de vehículo por condición** | Gráfico de barras apiladas comparando la condición de cada tipo de vehículo |

Todos los gráficos son interactivos (zoom, hover con detalles, filtros) gracias a Plotly.

---

## 📦 Dataset

El dataset contiene anuncios de venta de vehículos en EE. UU., con variables como:

`price` · `model_year` · `model` · `condition` · `cylinders` · `fuel` · `odometer` · `transmission` · `type` · `paint_color` · `is_4wd`

> Coloca el CSV del dataset en la ruta que espera la app (ver [Estructura del repositorio](#-estructura-del-repositorio)) antes de ejecutarla localmente.

---

## 🛠️ Tecnologías

- Python 3.9+
- [Streamlit](https://streamlit.io/) — interfaz web interactiva
- [Plotly](https://plotly.com/python/) — visualizaciones dinámicas
- pandas — manipulación de datos

---

## 🚀 Instalación y uso local

```bash
# clonar el repositorio
git clone <url-del-repo>
cd <nombre-del-repo>

# crear entorno virtual (opcional pero recomendado)
python -m venv venv
source venv/bin/activate      # en Windows: venv\Scripts\activate

# instalar dependencias
pip install -r requirements.txt

# ejecutar la app
streamlit run app.py
```

La app se abrirá automáticamente en `http://localhost:8501`.

---

## 📁 Estructura del repositorio

```
├── README.md
├── requirements.txt
├── app.py                 # aplicación principal de Streamlit
└── vehicles_us.csv        # dataset de anuncios de vehículos
```
