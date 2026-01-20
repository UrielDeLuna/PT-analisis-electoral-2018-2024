# Documento 04 – Reglas de Normalización de la Dimensión Sección Electoral

## 1. Alcance
Este documento define las reglas de normalización aplicables a la dimensión territorial de sección electoral (`DIM_SECCION`).

Las reglas aquí establecidas deberán aplicarse a todos los procesos de transformación de datos relacionados con secciones electorales dentro del proyecto.

---

## 2. Normalización de nombres de columnas

Las columnas deberán cumplir las siguientes reglas:

- Uso exclusivo de minúsculas
- Sin acentos
- Sin espacios (usar guiones bajos)
- Nombres descriptivos y consistentes

Ejemplo:

| Original | Normalizado |
|--------|------------|
| Nombre de Municipio | municipio |
| Distrito Federal | distrito_federal |
| Tipo de Sección | tipo_seccion |

---

## 3. Normalización de valores categóricos

Los valores categóricos deberán utilizar catálogos cerrados.

### Tipo de sección

Valores permitidos:

- URBANO
- RURAL
- MIXTO

No se permiten variantes ortográficas o de capitalización.

---

## 4. Normalización de claves

Las siguientes claves serán utilizadas como identificadores:

- `clave_entidad`
- `clave_municipio`
- `seccion`
- `distrito_federal`

Los nombres descriptivos (entidad, municipio) no serán utilizados como claves primarias.

---

## 5. Manejo de valores nulos

- Los valores faltantes deberán representarse como `NULL`
- No se utilizarán cadenas vacías ni valores como "N/A"

---

## 6. Resultado esperado

El resultado del proceso de normalización será una tabla limpia y consistente denominada:

DIM_SECCION_CDMX_2024

La cual se almacenará en el directorio:

data/processed/

