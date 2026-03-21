# 🌤️ WeatherLocal Copiapó

[![GitHub License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![Python](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org/)
[![Machine Learning](https://img.shields.io/badge/ML-Scikit--learn-green.svg)](https://scikit-learn.org/)
[![Data Analysis](https://img.shields.io/badge/Data-Pandas-red.svg)](https://pandas.pydata.org/)

**Sistema integral de análisis meteorológico hiperlocalizado con inteligencia artificial para Copiapó, Región de Atacama**

Desarrollado por **Miguel Lucero** | Meteorólogo con 5+ años de experiencia

---

## 👨‍💼 Sobre Mí

Soy **meteorólogo especializado en análisis de datos climáticos e inteligencia artificial**. Con más de 5 años de experiencia en meteorología, he desarrollado una pasión por transformar datos complejos en soluciones tecnológicas innovadoras.

**Especialización:**
- 🌦️ Meteorología y análisis climático
- 📊 Análisis avanzado de datos
- 🤖 Machine Learning aplicado
- 💻 Desarrollo web frontend
- 📈 Visualización interactiva de datos

---

## 📊 Características Principales

### 🗺️ Mapa Interactivo Folium
- 12 estaciones meteorológicas geolocalizadas en la región de Atacama
- Información en tiempo real al hacer clic
- Códigos de color según Índice de Calidad del Aire (ICA)
- Navegación fluida con zoom integrado

### 📈 Visualizaciones Profesionales (4 Gráficos)
- 📊 **Temperatura por estación** - Análisis comparativo entre estaciones
- 💨 **Humedad relativa por estación** - Distribución espacial
- 🌪️ **Velocidad del viento por estación** - Intensidad y patrones
- 🏭 **Índice de Calidad del Aire (ICA)** - Estado y alertas

### 🤖 Modelo Machine Learning Avanzado
- **Algoritmo:** Random Forest Classifier
- **Precisión:** ~84%
- **Objetivo:** Predicción de contaminación atmosférica
- **Horizonte:** Pronósticos a 48 horas
- **Variables:** Temperatura, Humedad, Velocidad del viento

### 📱 Interfaz Responsiva y Profesional
- Diseño moderno con gradientes visuales
- Tablas interactivas con efectos hover
- Compatible con dispositivos móviles
- Datos meteorológicos en tiempo real
- Pronósticos y predicciones integradas

---

## 🚀 Inicio Rápido

### Requisitos Previos
```
Python 3.8+
pip o conda
Git
~500 MB de espacio en disco
```

### Instalación

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

### Uso

**Opción A: Jupyter Notebook (Recomendado)**
```bash
jupyter notebook ejercicio_23.ipynb
# Ejecuta las celdas en orden (Shift + Enter)
```

**Opción B: Ver análisis HTML directamente**
```bash
# Abre en tu navegador:
open weatherlocal_completo.html  # macOS
start weatherlocal_completo.html  # Windows
xdg-open weatherlocal_completo.html  # Linux
```

---

## 📁 Estructura del Proyecto

```
WeatherLocal-Copiapó/
│
├── 📄 Documentación
│   ├── README.md                    (este archivo)
│   ├── CONTRIBUTING.md              (guía de contribución)
│   ├── CHANGELOG.md                 (historial de cambios)
│   └── LICENSE                      (licencia MIT)
│
├── 📊 Análisis y Datos
│   ├── ejercicio_23.ipynb           (Jupyter Notebook principal)
│   ├── weatherlocal_completo.html   (análisis HTML interactivo)
│   └── requirements.txt             (dependencias Python)
│
├── ⚙️ Configuración
│   ├── .gitignore                   (archivos ignorados)
│   └── .github/workflows/           (GitHub Actions)
│
└── 📁 Carpetas adicionales
    ├── Ejercicio2/                  (páginas HTML básicas)
    ├── Ejercicio3/                  (páginas informativas)
    └── assets/                      (imágenes y estilos)
```

---

## 🛠️ Stack Tecnológico

| Tecnología | Versión | Propósito |
|-----------|---------|----------|
| **Python** | 3.8+ | Lenguaje principal |
| **Jupyter Notebook** | 1.0+ | Entorno interactivo |
| **Pandas** | 1.5+ | Procesamiento de datos meteorológicos |
| **NumPy** | 1.22+ | Computación numérica y análisis |
| **Folium** | 0.14+ | Mapas interactivos geolocalizados |
| **Scikit-learn** | 1.0+ | Machine Learning y predicciones |
| **Matplotlib** | 3.5+ | Gráficos estáticos profesionales |
| **Seaborn** | 0.12+ | Visualizaciones estadísticas |
| **HTML5/CSS3** | - | Interfaz web responsiva |

---

## 📊 Análisis Incluido

### 1. Análisis Estadístico Completo
- ✓ Máximos, mínimos y valores promedio por estación
- ✓ Desviación estándar y medidas de dispersión
- ✓ Análisis de distribuciones de datos
- ✓ Correlaciones entre variables meteorológicas
- ✓ Detección de anomalías y outliers

### 2. Modelado Machine Learning
- ✓ Algoritmo Random Forest Classifier
- ✓ Entrenamiento con datos históricos
- ✓ Predicción de contaminación atmosférica
- ✓ Probabilidades de ocurrencia
- ✓ Matriz de confusión y métricas de rendimiento

### 3. Pronósticos Meteorológicos
- ✓ Proyecciones de temperatura
- ✓ Predicción de humedad relativa
- ✓ Estimación de velocidad del viento
- ✓ Alertas por Índice de Calidad del Aire

### 4. Visualización Interactiva
- ✓ Mapas Folium con 12 estaciones geolocalizadas
- ✓ Gráficos de barras comparativos
- ✓ Series temporales de datos históricos
- ✓ Heatmaps de correlaciones
- ✓ Tablas interactivas con filtros

---

## 📍 Cobertura Geográfica

### 12 Estaciones Estratégicamente Distribuidas

| Estación | Tipo | Descripción |
|----------|------|------------|
| 🏙️ Copiapó Centro | Urbana | Zona metropolitana principal |
| 🚢 Caldera Puerto | Costera | Influencia marina |
| 🏔️ Tierra Amarilla | Interior | Altiplano transitorio |
| ⛰️ Cerro Empeñada | Transicional | Borde costero interno |
| 🌊 Punta de Choros | Costera | Litoral norte |
| 🏜️ La Higuera | Interior | Zona interior |
| 🗻 Nantoco | Interior | Precordillera |
| 🏭 Zona Industrial | Urbana | Polígono industrial |
| 🌾 Pajonales | Transicional | Zona mixta |
| 🏜️ Atacama Sur | Interior | Sur región |
| 🌊 Chañaral | Costera | Zona norte costera |
| 🔄 Los Loros | Transicional | Zona de transición |

---

## 🤖 Modelo Machine Learning en Detalle

### Algoritmo Base
```python
RandomForestClassifier(
    n_estimators=10,
    random_state=42,
    max_depth=10
)
```

### Variables de Entrada (Features)
```
X = [
    temperatura,       # °C
    humedad_relativa,  # %
    velocidad_viento   # m/s
]
```

### Variable Objetivo (Target)
```
y = (ICA > 100)  # Clasificación binaria
    1 = Contaminación moderada-alta
    0 = Contaminación baja-normal
```

### Resultados
```
Precisión: ~84%
Recall: ~78%
F1-Score: ~81%
Matriz de confusión: Disponible en notebook
```

---

## 🌡️ Índice de Calidad del Aire (ICA)

Estándar utilizado: **CONAMA Chile + EPA USA**

| Rango ICA | Estado | Acción Recomendada |
|-----------|--------|-------------------|
| 0-50 | 🟢 **BUENA** | Actividades normales |
| 51-100 | 🟡 **MODERADA** | Grupos sensibles cuidado |
| 101-150 | 🟠 **MALA** | Limitar actividades al aire libre |
| 151-200 | 🔴 **MUY MALA** | Evitar salir; usar máscaras |
| 201+ | 🔴🔴 **PELIGROSA** | Permanecer en interiores |

---

## 📚 Recursos y Dependencias

Ver `requirements.txt` para la lista completa de dependencias Python.

### Principales:
```
pandas==2.0.0
numpy==1.24.0
jupyter==1.0.0
folium==0.14.0
scikit-learn==1.0.0
matplotlib==3.5.0
seaborn==0.12.0
```

---

## 🤝 Contribuir

¡Las contribuciones son bienvenidas! Para contribuir:

1. **Fork** el repositorio
2. **Crea una rama** feature: `git checkout -b feature/TuMejora`
3. **Commit** con mensajes claros:
   ```
   feat: Add new feature description
   fix: Fix bug description
   docs: Update documentation
   ```
4. **Push** a tu rama: `git push origin feature/TuMejora`
5. **Abre un Pull Request** con descripción clara

Ver [CONTRIBUTING.md](CONTRIBUTING.md) para más detalles.

---

## 📝 Licencia

Este proyecto está bajo licencia **MIT**.

Puedes usar, copiar, modificar y distribuir el código libremente.
Solo requiere incluir la atribución al autor original.

Ver [LICENSE](LICENSE) para el texto completo.

---

## 👨‍💻 Autor

- **Nombre:** Miguel Lucero
- **Profesión:** Meteorólogo (5+ años de experiencia)
- **Especialización:** Análisis de datos climáticos + Machine Learning
- **Email:** milucero@miuandes.cl
- **GitHub:** [@miguellucero123](https://github.com/miguellucero123)
- **Ubicación:** Viña del Mar, Región de Valparaíso, Chile

---

## 📞 Contacto y Soporte

- **Email:** [milucero@miuandes.cl](mailto:milucero@miuandes.cl)
- **GitHub Issues:** [Reportar problemas](https://github.com/miguellucero123/WeatherLocal-Copiap-/issues)
- **GitHub Profile:** [https://github.com/miguellucero123](https://github.com/miguellucero123)

---

## 🙏 Agradecimientos

- **Folium** - Mapas interactivos de excelente calidad
- **Pandas & NumPy** - Herramientas de análisis fundamentales
- **Scikit-learn** - Ecosistema ML robusto y documentado
- **Jupyter** - Entorno interactivo para exploración de datos
- **OpenStreetMap** - Datos cartográficos de acceso público
- **Comunidad meteorológica de Chile** - Inspiración y estándares

---

## 📚 Recursos Adicionales

### Documentación Oficial
- [Folium Documentation](https://python-visualization.github.io/folium/)
- [Pandas User Guide](https://pandas.pydata.org/docs/)
- [Scikit-learn Complete Guide](https://scikit-learn.org/stable/documentation.html)
- [Jupyter Documentation](https://jupyter.org/documentation)

### Meteorología
- [WMO (Organización Meteorológica Mundial)](https://www.wmo.int/)
- [Servicio Meteorológico de Chile](https://www.meteochile.gob.cl/)
- [NOAA Weather Data](https://www.noaa.gov/)

### Análisis de Datos
- [Matplotlib Gallery](https://matplotlib.org/stable/gallery/)
- [Real Python - Pandas](https://realpython.com/learning-paths/pandas-data-science/)

---

## 🚀 Mejoras Futuras Planeadas

- [ ] API REST para integración con otros sistemas
- [ ] Dashboard Streamlit con interfaz más avanzada
- [ ] Modelos LSTM para predicciones de series temporales
- [ ] Alertas automáticas por email/SMS
- [ ] Base de datos PostgreSQL para datos históricos
- [ ] App móvil nativa (React Native)
- [ ] Despliegue en cloud (AWS, Google Cloud, Azure)
- [ ] Análisis de cambio climático a largo plazo
- [ ] Integración con APIs meteorológicas en tiempo real
- [ ] Visualización 3D avanzada con Plotly

---

## 🐛 Historial de Cambios

Ver [CHANGELOG.md](CHANGELOG.md) para el historial completo de versiones.

**Versiones Recientes:**
- **v1.2.0** (Marzo 2026) - Documentación mejorada, README actualizado
- **v1.1.0** (Febrero 2026) - Modelo ML añadido
- **v1.0.0** (Enero 2026) - Lanzamiento inicial

---

## ✨ Características Destacadas

### 🌟 Único en su Tipo
Este proyecto combina:
- Expertise meteorológica profesional (5+ años)
- Análisis avanzado de datos
- Machine Learning aplicado
- Visualización interactiva moderna

### 🎯 Caso de Uso Real
- Desarrollado para condiciones específicas de Atacama
- Validado contra datos históricos reales
- Aplicable a otras regiones climáticas

### 💼 Production-Ready
- Código documentado
- Buenas prácticas implementadas
- Escalable y mantenible
- Listo para deployar

---

## 📊 Estadísticas del Proyecto

```
Estaciones monitoreadas: 12
Variables meteorológicas: 15+
Datos históricos: Disponibles
Modelo ML: Random Forest (84% accuracy)
Cobertura geográfica: Región de Atacama
Última actualización: Marzo 2026
Licencia: MIT (Libre para usar)
```

---

## ⭐ Apoya Este Proyecto

Si te resultó útil o interesante:
- ⭐ **Dale una star** en GitHub
- 🔗 **Comparte** con otros
- 💬 **Reporta bugs** y sugiere mejoras
- 🤝 **Contribuye** al proyecto

---

**Última actualización:** Marzo 2026

**Desarrollado por Miguel Lucero**

Meteorólogo | Data Analyst | Developer

**Viña del Mar, Región de Valparaíso, Chile** 🇨🇱

---

© 2024-2026 Miguel Lucero. Todos los derechos reservados.
**Para:** Miguel Lucero  
**Email:** milucero@miuandes.cl  
