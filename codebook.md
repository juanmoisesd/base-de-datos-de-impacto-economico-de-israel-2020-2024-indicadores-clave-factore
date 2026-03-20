# Codebook — Base de Datos de Impacto Económico de Israel (2020–2024)

## 1. Descripción General

Este documento describe la estructura, variables, definiciones y características técnicas del dataset:

**“Base de Datos de Impacto Económico de Israel (2020–2024)”**

El dataset integra indicadores macroeconómicos, financieros y geopolíticos con el objetivo de facilitar análisis económicos, estudios comparativos y evaluación de impacto de eventos en el periodo 2020–2024.

---

## 2. Cobertura

| Dimensión        | Descripción |
|------------------|------------|
| País             | Israel |
| Periodo          | 2020–2024 |
| Frecuencia       | Anual (principal) / Mixta (según variable) |
| Unidades         | %, USD, índice base, valores absolutos |
| Tipo de datos    | Series temporales estructuradas |
| Número de tablas | 9 |

---

## 3. Estructura del Dataset

El dataset se divide en 9 tablas temáticas independientes pero relacionadas.

---

## 4. Diccionario de Variables

### 4.1 Tabla 1 – Indicadores Macroeconómicos Anuales

| Variable               | Tipo    | Unidad | Descripción |
|------------------------|--------|--------|------------|
| year                   | Integer | Año | Año de referencia |
| gdp_real_growth        | Float   | % | Crecimiento real del PIB |
| inflation_cpi          | Float   | % | Inflación anual (Índice de Precios al Consumidor) |
| unemployment_rate      | Float   | % | Tasa de desempleo |

---

### 4.2 Tabla 2 – Sector Externo y Comercio

| Variable                    | Tipo  | Unidad | Descripción |
|-----------------------------|------|--------|------------|
| exports_goods_services      | Float | USD (millones) | Exportaciones totales |
| imports_goods_services      | Float | USD (millones) | Importaciones totales |
| current_account_balance     | Float | % PIB | Saldo de cuenta corriente |

---

### 4.3 Tabla 3 – Finanzas Públicas

| Variable               | Tipo  | Unidad | Descripción |
|------------------------|------|--------|------------|
| fiscal_balance_gdp     | Float | % PIB | Balance fiscal |
| public_debt_gdp        | Float | % PIB | Deuda pública |
| government_expenditure | Float | % PIB | Gasto público |

---

### 4.4 Tabla 4 – Mercado Laboral y Salarios

| Variable                    | Tipo  | Unidad | Descripción |
|-----------------------------|------|--------|------------|
| employment_rate            | Float | % | Tasa de empleo |
| labor_force_participation  | Float | % | Participación laboral |
| average_wage_index         | Float | Índice | Índice de salario medio |

---

### 4.5 Tabla 5 – Precios, Vivienda y Consumo

| Variable                    | Tipo  | Unidad | Descripción |
|-----------------------------|------|--------|------------|
| housing_price_index        | Float | Índice | Índice de precios de vivienda |
| rent_price_index           | Float | Índice | Índice de alquiler |
| private_consumption_growth | Float | % | Crecimiento del consumo privado |

---

### 4.6 Tabla 6 – Sistema Financiero e Índices de Mercado

| Variable                  | Tipo  | Unidad | Descripción |
|---------------------------|------|--------|------------|
| policy_interest_rate      | Float | % | Tipo de interés oficial |
| stock_index_ta35          | Float | Índice | Índice bursátil TA-35 |
| credit_to_private_sector  | Float | % PIB | Crédito al sector privado |

---

### 4.7 Tabla 7 – Tipo de Cambio y Sector Externo Financiero

| Variable              | Tipo  | Unidad | Descripción |
|------------------------|------|--------|------------|
| exchange_rate_usd_ils | Float | ILS/USD | Tipo de cambio |
| foreign_reserves      | Float | USD (millones) | Reservas internacionales |
| net_fdi_flows         | Float | USD (millones) | Flujos netos de inversión extranjera |

---

### 4.8 Tabla 8 – Riesgo País

| Variable          | Tipo  | Unidad | Descripción |
|------------------|------|--------|------------|
| sovereign_spread | Float | Puntos básicos | Prima de riesgo soberano |
| credit_rating    | String | Categoría | Calificación crediticia |
| cds_5y           | Float | Puntos básicos | CDS a 5 años |

---

### 4.9 Tabla 9 – Shocks Geopolíticos

| Variable                   | Tipo   | Unidad | Descripción |
|----------------------------|--------|--------|------------|
| event_date                | Date   | Fecha | Fecha del evento |
| event_type                | String | Categoría | Tipo de evento |
| conflict_intensity_index  | Float  | Índice | Intensidad del conflicto |
| policy_response_dummy     | Integer| 0/1 | Respuesta política (dummy) |

---

## 5. Fuentes de Datos

Los datos provienen de fuentes institucionales y bases económicas reconocidas:

- World Bank  
- International Monetary Fund (IMF)  
- OECD  
- Bank of Israel  
- Trading Economics  

Se ha aplicado validación cruzada entre fuentes cuando ha sido posible.

---

## 6. Procesamiento de Datos

El dataset ha sido sometido a los siguientes procesos:

- Normalización de unidades
- Estandarización de nombres de variables
- Eliminación de inconsistencias
- Conversión a formato estructurado
- Integración de múltiples fuentes

---

## 7. Consideraciones Metodológicas

- Algunas variables presentan diferencias de frecuencia (anual vs mensual agregada).
- Los índices pueden estar normalizados con bases distintas según fuente original.
- Variables geopolíticas han sido operacionalizadas mediante proxies (ej. índices de intensidad).

---

## 8. Limitaciones

- Posibles discrepancias entre fuentes originales
- Falta de disponibilidad homogénea en algunas variables
- Simplificación de eventos geopolíticos complejos

---

## 9. Uso Recomendado

Este dataset es adecuado para:

- Modelos econométricos
- Análisis de series temporales
- Estudios geoeconómicos
- Evaluación de impacto de conflictos
- Investigación académica

---

## 10. Citación


de la Serna Tuya, J. M. (2026). Base de Datos de Impacto Económico de Israel (2020–2024). Zenodo. https://doi.org/10.5281/zenodo.18879626


---

## 11. Contacto

Juan Moisés de la Serna Tuya  
ORCID: https://orcid.org/0000-0002-8401-8018  
Web: https://juanmoisesdelaserna.es  
