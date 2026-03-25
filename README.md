# Análisis de la Esperanza de Vida y Mortalidad a Nivel Global

Estudio realizado con R y RStudio sobre los determinantes y tendencias que influyen en la esperanza de vida y la mortalidad a nivel mundial. El análisis explora cómo factores nutricionales, causas de muerte, elementos económicos y acceso a recursos básicos han afectado estas métricas a lo largo del tiempo en distintas regiones del mundo.

**Autor:** Álvaro Rodríguez González  
**Fecha:** Mayo 2024

---

## Contenido del repositorio

```
life-expectancy-study/
├── report/
│   ├── memoria.Rmd       # Informe principal
│   ├── memoria.html      # Informe renderizado
│   ├── prueba.Rmd        # Cuadro de mandos (Shiny/flexdashboard)
│   └── styles2.css       # Estilos del informe
└── data/
    ├── life-expectancy.csv
    ├── life-expectancy-vs-gdp-per-capita.csv
    ├── life-expectancy-vs-healthcare-expenditure.csv
    ├── life-expectation-at-birth-by-sex.csv
    ├── annual-number-of-deaths-by-cause.csv
    ├── annual-death-rates-in-different-age-groups.csv
    ├── age-standardized-deaths-from-all-causes.csv
    ├── prevalence-of-undernourishment.csv
    ├── inseguridad-alimentaria-paises.csv
    ├── obesidad-paises.csv
    ├── water-and-sanitation.csv
    └── geo_countries.geojson
```

---

## Fuentes de datos

- **[Our World in Data (OWID)](https://ourworldindata.org/)** — esperanza de vida, mortalidad y causas de muerte.
- **[FAO](https://www.fao.org/home/en/)** — inseguridad alimentaria y nutrición mundial.

---

## Tecnologías utilizadas

- **R / RStudio**
- **RMarkdown** — para el informe y el cuadro de mandos
- **Highcharter** — visualizaciones dinámicas e interactivas
- **flexdashboard** — cuadro de mandos
- **ggplot2 / plotly** — gráficos complementarios
- **fpp3** — análisis de series temporales

---

## Cómo reproducir el informe

Con RStudio abierto en la raíz del proyecto:

```r
rmarkdown::render("report/memoria.Rmd")
```

Las dependencias se instalan automáticamente al ejecutar el informe si no están disponibles.

---

## Principales hallazgos

- El **PIB per cápita y la inversión en salud pública** muestran una correlación positiva con la esperanza de vida a largo plazo.
- El **acceso a agua potable** es uno de los factores con mayor correlación positiva con la longevidad.
- Las **enfermedades cardiovasculares y el cáncer** son las principales causas de muerte a nivel global.
- La **inseguridad alimentaria** muestra una correlación baja con el resto de variables analizadas.
- Se observa una anomalía en la mortalidad de 1950 atribuible a los efectos prolongados de la Segunda Guerra Mundial.
