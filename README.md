# 📱 Sprint 11 – Proyecto Final: Análisis de Comportamiento de Usuario en App de Alimentos

Este proyecto forma parte del curso *"La toma de decisiones de negocios basadas en datos"* y tiene como objetivo analizar el comportamiento de los usuarios dentro de una aplicación de venta de productos alimenticios. Incluye un estudio del embudo de eventos y el análisis de un experimento A/A/B para evaluar cambios en la interfaz de usuario.

---

## 🎯 Objetivos del Proyecto

- Analizar el *embudo de conversión* dentro de la aplicación.
- Determinar puntos críticos donde los usuarios abandonan el proceso.
- Evaluar el impacto de un cambio de diseño (tipografía) mediante un *test A/A/B*.
- Verificar la validez del experimento mediante análisis de significancia estadística.

---

## 📁 Dataset

- *logs_exp_us.csv*  
  Contiene registros de eventos realizados por los usuarios de la aplicación:

  | Columna         | Descripción |
  |-----------------|-------------|
  | EventName     | Nombre del evento realizado por el usuario |
  | DeviceIDHash  | Identificador único del usuario |
  | EventTimestamp| Fecha y hora del evento |
  | ExpId         | Grupo experimental (246, 247: control; 248: prueba) |

---

## 🔍 Estructura del análisis

### 1. Preprocesamiento
- Renombrado de columnas.
- Conversión de tipos de datos.
- Creación de columnas de fecha y hora separadas.

### 2. Exploración de datos
- Conteo de eventos y usuarios únicos.
- Eventos promedio por usuario.
- Identificación del periodo válido para análisis.
- Verificación de la distribución de usuarios por grupo experimental.

### 3. Análisis del embudo
- Frecuencia de eventos.
- Porcentaje de usuarios por evento.
- Conversión por etapas del embudo.
- Detección de puntos de fuga de usuarios.

### 4. Análisis del test A/A/B
- Comparación entre grupos de control (246 vs. 247).
- Pruebas de significancia para cada evento entre grupos.
- Evaluación del grupo experimental (248) vs. grupos control.
- Aplicación de corrección por múltiples pruebas (nivel de significancia).

---

## 🛠️ Herramientas utilizadas

- *Python*: pandas, numpy, scipy, matplotlib, seaborn  
- *Estadística*: pruebas de hipótesis, proporciones, validación experimental  
- *Visualización*: histogramas, embudos, comparaciones entre grupos

---

## 📌 Resultados esperados

- Identificar los eventos más críticos para la conversión.
- Determinar si el nuevo diseño (tipografía) afecta positiva o negativamente el comportamiento del usuario.
- Validar que los grupos de control sean estadísticamente equivalentes.
- Emitir recomendaciones sobre la implementación del nuevo diseño.

---

## 👩‍⚕️ Autor

*[Tu Nombre]*  
Médica | Analista de datos en formación | Interesada en investigación interdisciplinaria  
🔗 [LinkedIn](https://www.linkedin.com/in/tu-usuario) | 💻 [GitHub](https://github.com/tu-usuario)

---

> Proyecto educativo – Parte del programa de Data Analysis for Business Decision-Making.
