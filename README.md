# 🌍 Global Carbon Pulse: Dashboard de Emisiones de CO₂ (1950-2024)

¡Bienvenido a mi proyecto de análisis de datos! Este repositorio contiene el desarrollo de un dashboard ejecutivo e interactivo en **Power BI** enfocado en la evolución histórica de las emisiones globales de dióxido de carbono ($CO_2$), utilizando datos públicos de *Our World in Data*.

---

## 📊 Vista Previa del Dashboard
<img width="1354" height="764" alt="image" src="https://github.com/user-attachments/assets/4a43f17b-4b21-4f76-b6a7-a2095476ebbd" />

---

## 🎯 Objetivos del Proyecto
* **Identificar focos críticos:** Mapear geográficamente los países con mayor volumen de emisiones.
* **Analizar tendencias temporales:** Evaluar la tasa de crecimiento anual global.
* **Desglosar la matriz energética:** Comprender el impacto individual del carbón, petróleo, gas y cemento en la crisis climática.

---

## 🛠️ Tecnologías y Herramientas Utilizadas
* **Figma / Canva:** Diseño de la interfaz de usuario (UI), layouts de tarjetas y fondos con contraste `#F8F9FA`.
* **SQL:** Extracción, limpieza preliminar y consultas analíticas del dataset.
* **Power BI Desktop:** Modelado de datos, relaciones y creación de medidas analíticas con DAX.
* **JSON:** Configuración de un tema visual nativo personalizado.

---

## 📐 Fórmulas DAX Destacadas

Para asegurar que el dashboard sea interactivo y dinámico ante los filtros del usuario, desarrollé medidas avanzadas con control de configuración regional en español:

* **Emisiones Totales:**
  ```dax
  Emisiones Totales = SUM('DATA'[co2])
