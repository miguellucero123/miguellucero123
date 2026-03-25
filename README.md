# WeatherLocal Copiapó

[![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![Python](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org/)
[![Scikit-learn](https://img.shields.io/badge/ML-Scikit--learn-green.svg)](https://scikit-learn.org/)

Sistema integral de análisis meteorológico hiperlocalizado con aprendizaje automático para la Región de Atacama, Chile.

**Autor:** Miguel Lucero — Meteorólogo, analista de datos climáticos

---

## Descripción

WeatherLocal Copiapó integra datos de una red de 12 estaciones meteorológicas distribuidas estratégicamente en la Región de Atacama. El sistema combina análisis estadístico exploratorio, visualización geoespacial interactiva y un modelo de clasificación supervisada para la predicción del Índice de Calidad del Aire (ICA) con un horizonte de 48 horas.

El proyecto está diseñado para ser reproducible, documentado y escalable, siguiendo buenas prácticas de ciencia de datos aplicada a la meteorología regional.

---

## Funcionalidades Principales

### Visualización geoespacial
- Mapa interactivo (Folium/OpenStreetMap) con 12 estaciones geolocalizadas
- Codificación cromática basada en el ICA (estándar CONAMA Chile / EPA USA)
- Información meteorológica en tiempo real por estación al interactuar con el mapa

### Análisis estadístico
- Estadísticas descriptivas por estación: media, desviación estándar, mínimo, máximo
- Análisis de distribuciones y detección de valores atípicos
- Matrices de correlación entre variables meteorológicas

### Visualizaciones analíticas
Cuatro gráficos comparativos entre estaciones:
1. Temperatura del aire (°C)
2. Humedad relativa (%)
3. Velocidad del viento (m/s)
4. Índice de Calidad del Aire (ICA)

### Modelo de aprendizaje automático
- **Algoritmo:** Random Forest Classifier
- **Variables predictoras:** temperatura, humedad relativa, velocidad del viento
- **Variable objetivo:** clasificación binaria de contaminación (ICA > 100)
- **Métricas de evaluación:** precisión ~84%, recall ~78%, F1-score ~81%
- **Horizonte de predicción:** 48 horas

---

## Instalación

### Requisitos previos

- Python 3.8 o superior
- pip o conda
- Git
- ~500 MB de espacio en disco

### Pasos

```bash
# 1. Clonar el repositorio
git clone https://github.com/miguellucero123/WeatherLocal-Copiap-.git
cd "WeatherLocal-Copiap-"

# 2. Crear entorno virtual (recomendado)
conda create -n weatherlocal python=3.11 -y
conda activate weatherlocal

# 3. Instalar dependencias
pip install -r requirements.txt
```

---

## Uso

**Opción A — Jupyter Notebook (recomendado):**
```bash
jupyter notebook ejercicio_23.ipynb
# Ejecutar las celdas en orden secuencial (Shift + Enter)
```

**Opción B — Análisis HTML estático:**
```bash
# Abrir directamente en el navegador:
open weatherlocal_completo.html        # macOS
start weatherlocal_completo.html       # Windows
xdg-open weatherlocal_completo.html    # Linux
```

---

## Estructura del Proyecto

```
WeatherLocal-Copiapó/
├── ejercicio_23.ipynb              # Notebook principal de análisis
├── weatherlocal_completo.html      # Informe HTML interactivo
├── requirements.txt                # Dependencias Python
├── README.md
├── CONTRIBUTING.md
├── CHANGELOG.md
├── LICENSE
├── .gitignore
├── .github/workflows/              # Integración continua (GitHub Actions)
├── Ejercicio2/                     # Páginas HTML auxiliares
├── Ejercicio3/                     # Páginas informativas
└── assets/                         # Recursos estáticos
```

---

## Dependencias

| Paquete | Versión mínima | Uso |
|---|---|---|
| pandas | 1.5 | Procesamiento de datos tabulares |
| numpy | 1.22 | Computación numérica |
| folium | 0.14 | Mapas interactivos georreferenciados |
| scikit-learn | 1.0 | Modelado de aprendizaje automático |
| matplotlib | 3.5 | Visualización estática |
| seaborn | 0.12 | Visualización estadística |
| jupyter | 1.0 | Entorno de análisis interactivo |

Véase `requirements.txt` para la lista completa con versiones exactas.

---

## Red de Estaciones

La red cubre un gradiente altitudinal y climático representativo de la región, desde la costa hasta la precordillera:

| Estación | Contexto geográfico |
|---|---|
| Copiapó Centro | Zona metropolitana principal |
| Caldera Puerto | Influencia marina directa |
| Tierra Amarilla | Altiplano transitorio interior |
| Cerro Empeñada | Borde costero interno |
| Punta de Choros | Litoral norte |
| La Higuera | Zona interior árida |
| Nantoco | Precordillera |
| Zona Industrial | Polígono industrial urbano |
| Pajonales | Zona mixta transicional |
| Atacama Sur | Sector sur de la región |
| Chañaral | Costa norte |
| Los Loros | Zona de transición climática |

---

## Modelo de Clasificación

```python
RandomForestClassifier(
    n_estimators=10,
    max_depth=10,
    random_state=42
)

# Variables de entrada (features)
X = ['temperatura',       # °C
     'humedad_relativa',  # %
     'velocidad_viento']  # m/s

# Variable objetivo (target) — clasificación binaria
y = (ICA > 100)
# 1: contaminación moderada a alta
# 0: contaminación baja o normal
```

**Resultados de evaluación:**

| Métrica | Valor |
|---|---|
| Accuracy | ~84% |
| Recall | ~78% |
| F1-score | ~81% |

La matriz de confusión completa está disponible en el notebook.

---

## Índice de Calidad del Aire (ICA)

Clasificación según estándar CONAMA Chile / EPA USA:

| Rango ICA | Categoría | Recomendación |
|---|---|---|
| 0–50 | Buena | Actividades normales |
| 51–100 | Moderada | Precaución para grupos sensibles |
| 101–150 | Mala | Limitar actividades al aire libre |
| 151–200 | Muy mala | Evitar exposición exterior |
| >200 | Peligrosa | Permanecer en interiores |

---

## Contribuciones

Las contribuciones son bienvenidas. Para contribuir:

1. Haz un fork del repositorio
2. Crea una rama con nombre descriptivo: `git checkout -b feature/nombre-mejora`
3. Realiza commits con mensajes claros siguiendo la convención:
   ```
   feat: descripción de la nueva funcionalidad
   fix: descripción de la corrección
   docs: actualización de documentación
   ```
4. Abre un Pull Request con descripción detallada del cambio

Consulta [CONTRIBUTING.md](CONTRIBUTING.md) para lineamientos completos.

---

## Trabajo Futuro

- API REST para integración con sistemas externos
- Dashboard interactivo con Streamlit
- Modelos LSTM para predicción de series temporales
- Alertas automáticas por correo y SMS
- Persistencia en base de datos PostgreSQL
- Integración con APIs meteorológicas en tiempo real (DMC, NOAA)
- Análisis de tendencias de cambio climático a largo plazo
- Despliegue en infraestructura de nube (AWS / GCP / Azure)

---

## Versiones

| Versión | Fecha | Descripción |
|---|---|---|
| v1.2.0 | Marzo 2026 | Documentación mejorada, README actualizado |
| v1.1.0 | Febrero 2026 | Incorporación del modelo de ML |
| v1.0.0 | Enero 2026 | Lanzamiento inicial |

Véase [CHANGELOG.md](CHANGELOG.md) para el historial completo.

---

## Licencia

Distribuido bajo licencia **MIT**. El uso, copia, modificación y distribución del código son libres con atribución al autor original. Véase [LICENSE](LICENSE) para el texto completo.

---

## Autor y Contacto

**Miguel Lucero**  
Meteorólogo | Analista de datos climáticos  
Viña del Mar, Región de Valparaíso, Chile

- Correo: [milucero@miuandes.cl](mailto:milucero@miuandes.cl)
- GitHub: [@miguellucero123](https://github.com/miguellucero123)
- Issues: [Reportar un problema](https://github.com/miguellucero123/WeatherLocal-Copiap-/issues)

---

## Referencias y Recursos

- [Folium — Python Visualization](https://python-visualization.github.io/folium/)
- [Scikit-learn — Machine Learning in Python](https://scikit-learn.org/stable/documentation.html)
- [Pandas User Guide](https://pandas.pydata.org/docs/)
- [Dirección Meteorológica de Chile](https://www.meteochile.gob.cl/)
- [Organización Meteorológica Mundial (WMO)](https://www.wmo.int/)
- [NOAA Climate Data](https://www.noaa.gov/)

---

*Última actualización: Marzo 2026*
