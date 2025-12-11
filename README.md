# 📊 Análisis de Evasión de Clientes - Telecom X

## 🎯 Descripción del Proyecto

Análisis completo de datos y exploración de factores que causan la evasión de clientes (Churn) en Telecom X. Este proyecto aplica técnicas de ETL, Análisis Exploratorio de Datos (EDA) y análisis estadístico para identificar patrones de comportamiento de clientes.

## 📈 Hallazgos Principales

- **Tasa de Churn:** 26.54% (1,869 de 7,043 clientes)
- **Factor más importante:** Tenure (duración del contrato)
  - Clientes que se van: 18 meses promedio
  - Clientes que se quedan: 37.6 meses promedio
  
- **Segundo factor:** Cargos mensuales
  - Clientes con cargos altos: mayor tendencia a irse
  - Paradoja: posible falta de valor percibido

- **Tercero factor:** Estado civil y dependientes
  - Sin pareja: 32.96% churn
  - Con pareja: 19.66% churn
  - Con dependientes: 15.45% churn (mayor retención)

## 🛠️ Tecnologías Utilizadas

- **Lenguaje:** Python 3
- **Librerías principales:**
  - `pandas` - Manipulación y análisis de datos
  - `numpy` - Operaciones numéricas
  - `matplotlib` y `seaborn` - Visualización de datos
  - `scipy` - Análisis estadístico

- **Entorno:** Google Colab 

## 📁 Estructura del Proyecto

```
Desafio_2_TelecomX/
├── TelecomX_LATAM.ipynb   # Notebook principal
├── README.md              # Este archivo
├── images                 # carpeta con las visualizaciones generadas
```

## 📊 Proceso Ejecutado

### 1. Extracción (Extract)
- Conexión a API de GitHub
- Descarga de datos JSON desde repositorio ingridcristh/challenge2-data-science-LATAM
- 7,267 registros de clientes

### 2. Transformación (Transform)
- Eliminación de 224 registros con valores inválidos en Churn
- Estandarización de valores categóricos
- Codificación de variables binarias (Yes/No → 1/0)
- One-Hot Encoding para variables categóricas múltiples
- Validación de tipos de datos

### 3. Carga (Load)
- Preparación de datos limpios para análisis
- 7,043 registros finales válidos

### 4. Análisis Exploratorio (EDA)
- Análisis univariado: distribuciones de variables
- Análisis bivariado: relaciones con Churn
- Análisis de correlaciones
- Generación de 9 visualizaciones estratégicas
- Análisis estadístico detallado

## 📊 Visualizaciones Generadas

1. **Distribución de Churn** - Proporción de clientes que se van
2. **Distribución de Tenure** - Meses de contrato de clientes
3. **Distribución de Cargos Mensuales** - Costos de servicios
4. **Tenure vs Churn** - Box plot comparativo
5. **Cargos Mensuales vs Churn** - Box plot comparativo
6. **Cargos Totales vs Churn** - Box plot comparativo
7. **Adultos Mayores vs Churn** - Análisis por edad
8. **Estado Civil vs Churn** - Análisis por pareja
9. **Tipo de Internet vs Churn** - Análisis por servicio
10. **Matriz de Correlación** - Heatmap de todas las variables

## 💡 Recomendaciones Estratégicas

### Corto Plazo (0-3 meses)
- Programa de bienvenida mejorado en primeros 3 meses
- Revisión de precios para planes >$75/mes
- Atención proactiva para adultos mayores

### Mediano Plazo (3-6 meses)
- Crear planes familiares con descuentos
- Sistema de alertas de churn predictivo
- Mejora de servicios adicionales

### Largo Plazo (6-12 meses)
- Programa de fidelización con rewards
- Plataforma digital mejorada
- Modelo predictivo de churn con Machine Learning

**Meta:** Reducir churn de 26.54% a 20% en 12 meses

## 🎓 Objetivos de Aprendizaje Alcanzados

✅ Importar y manipular datos desde una API  
✅ Aplicar conceptos de ETL (Extracción, Transformación, Carga)  
✅ Crear visualizaciones estratégicas  
✅ Realizar Análisis Exploratorio de Datos (EDA)  
✅ Identificar patrones y tendencias  
✅ Generar insights basados en datos  
✅ Formular recomendaciones estratégicas  

## 📖 Cómo Usar Este Proyecto

1. Abre el archivo `TelecomX_LATAM.ipynb`
2. Ejecuta todas las celdas secuencialmente
3. Observa las visualizaciones y análisis
4. Lee las conclusiones en la última sección

## 📊 Diccionario de Datos

- **customerID:** ID único del cliente
- **Churn:** Si el cliente abandonó (Yes/No)
- **customer_tenure:** Meses de contrato
- **account_Charges.Monthly:** Cargos mensuales
- **account_Charges.Total:** Gasto total acumulado
- **customer_Partner:** Tiene pareja (Yes/No)
- **customer_Dependents:** Tiene dependientes (Yes/No)
- **customer_SeniorCitizen:** Es adulto mayor (Yes/No)
- **internet_InternetService:** Tipo de servicio de internet
- **account_Contract:** Tipo de contrato
- [Ver archivo notebook para variable completa]

## 📞 Contexto

**Desafío:** Data Science - Programa One - Alura  
**Empresa:** Telecom X (simulada)  
**Problema:** Reducir evasión de clientes mediante análisis de datos  

## ✅ Estado del Proyecto

**Estado:** ✅ Completado  
**Fecha:** Diciembre 2024  
**Siguiente paso:** Implementación de modelo predictivo con Machine Learning

---

**Análisis realizado por:** Christian Javier Lemos  
**GitHub:** https://github.com/javito72/Desafio_2_TelecomX