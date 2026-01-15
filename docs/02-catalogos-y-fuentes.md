# 02 – Catálogos y fuentes de datos

## 📌 Objetivo del documento
Este documento describe los catálogos, fuentes oficiales y conjuntos de datos utilizados en el proyecto, así como la justificación técnica de su selección.

Su propósito es asegurar trazabilidad, reproducibilidad y claridad en el origen de la información empleada en el análisis.

---

## 🗂️ Catálogo de secciones electorales (CSEDEF)

### Nombre oficial
**Catálogo de Secciones Electorales con Distritos Electorales Federales (CSEDEF)**

### Institución responsable
Instituto Nacional Electoral (INE)

### Descripción general
El CSEDEF es el listado oficial de las secciones electorales del país. Contiene información territorial y administrativa que permite identificar la relación entre secciones electorales, entidades federativas, distritos electorales federales y municipios (o alcaldías, en el caso de la Ciudad de México).

### Campos principales
- Clave de entidad federativa  
- Nombre de la entidad  
- Distrito electoral federal  
- Clave de municipio / alcaldía  
- Nombre de municipio / alcaldía  
- Sección electoral  
- Tipo de sección (urbana, rural o mixta)

---

## 🌎 Cobertura seleccionada

### Cobertura territorial
**Ciudad de México**

### Justificación
La cobertura de Ciudad de México permite:
- Reducir el volumen inicial de datos
- Facilitar el aprendizaje y control del procesamiento
- Realizar análisis territoriales detallados a nivel sección, distrito y alcaldía
- Construir visualizaciones cartográficas manejables

El diseño del proyecto permite escalar posteriormente a cobertura nacional utilizando el mismo catálogo.

---

## 📁 Formato de archivo

### Formato seleccionado
**Microsoft Excel (XLS)**

### Justificación
- Permite inspección visual directa del catálogo
- Compatible con herramientas de análisis como Excel, Power BI y Python
- Facilita procesos de limpieza y homologación de datos

---

## 🔗 Relación con otros conjuntos de datos

El catálogo CSEDEF será utilizado como tabla dimensional para:
- Vincular resultados electorales por sección
- Integrar geometrías territoriales (KML / SHP)
- Permitir agregaciones por distrito electoral y alcaldía

La clave principal de relación será la **sección electoral**.

---

## 📌 Rol del catálogo en el modelo de datos

Dentro del modelo de datos del proyecto, el CSEDEF cumple el rol de:

**DIM_SECCION**

Esta dimensión permitirá estructurar y organizar la información electoral y geográfica en etapas posteriores del análisis.
