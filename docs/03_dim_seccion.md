# Documento 03 – Definición de la Dimensión Sección Electoral

## 1. Propósito del documento
Este documento define la dimensión territorial de sección electoral que será utilizada como base para el análisis electoral del proyecto.

La dimensión permitirá agrupar, filtrar y relacionar resultados electorales con unidades territoriales oficiales.

---

## 2. Fuente de datos

- Fuente: Instituto Nacional Electoral (INE)
- Producto: Catálogo de Secciones Electorales con Distritos Electorales Federales (CSEDEF)
- Corte: Junio 2024
- Cobertura: Ciudad de México
- Formato original: Microsoft Excel (.xls)

Nombre original del archivo:
- Catalogo de Secciones.xls

Nombre interno en el proyecto:
- CSEDEF_CDMX_2024.xls

---

## 3. Ubicación del archivo

El archivo fuente se encuentra almacenado en:


## 4. Nivel de agregación

La dimensión se construirá a nivel de:

- Entidad federativa
- Alcaldía (municipio)
- Distrito electoral federal
- Sección electoral

---

## 5. Uso previsto

La dimensión `DIM_SECCION` será utilizada para:

- Relacionar resultados electorales (FACT_)
- Vincular información geográfica (MAP_)
- Soportar análisis por nivel territorial
- Construcción de visualizaciones en Power BI

