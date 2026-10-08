# 🏭 Análisis de OEE y Tiempos de Paro (Downtime) en Power BI

Este proyecto es un dashboard interactivo desarrollado en Power BI para monitorizar la Eficiencia General de los Equipos (OEE) y analizar los tiempos de inactividad en una planta de producción.

### 📸 Vistas del Dashboard
![Vista 1](Captura%20de%20pantalla%202026-10-08%20173526.png)
![Vista 2](Captura%20de%20pantalla%202026-10-08%20173557.png)
![Vista 3](Captura%20de%20pantalla%202026-10-08%20173626.png)

## 📌 Objetivo del Proyecto
Proporcionar a los gerentes de planta una herramienta dinámica para identificar cuellos de botella, analizar las causas raíz de los paros y evaluar el rendimiento de la maquinaria a través de indicadores clave (KPIs) como MTBF y MTTR.

## 🛠️ Herramientas y Técnicas Utilizadas
* **Power BI & DAX**: Creación de medidas complejas para inteligencia de tiempo y KPIs industriales.
* **Parámetros de Campo (Field Parameters)**: Implementados para permitir al usuario alternar dinámicamente las dimensiones (ej. Tipo de Máquina vs. Incidente) y métricas (MTBF vs. MTTR) en los mismos gráficos, optimizando el espacio visual.
* **Gráficos SVG Personalizados**: Generación de donas radiales mediante código SVG incrustado en medidas DAX para los porcentajes de progreso.
* **Modelado de Datos**: Esquema en estrella con tablas de dimensiones (`dim_machine`, `dim_incident`, `dim_date`, `dim_time`) conectadas a la tabla de hechos de producción. Relaciones de granularidad de tiempo ajustadas para análisis por turnos (AM/PM).

## 📊 Indicadores Clave (KPIs)
* **OEE (Overall Equipment Effectiveness)**: Disponibilidad, Rendimiento y Calidad.
* **MTBF (Mean Time Between Failures)**: Tiempo Medio Entre Fallas, con formato condicional.
* **MTTR (Mean Time To Repair)**: Tiempo Medio de Reparación.
* **Análisis de Paros**: Desglose dinámico de horas perdidas por causas como "Cambio y Limpieza", "Falta de Pedido" o "Mantenimiento Preventivo".

## 🚀 Cómo usar este proyecto
1. Descarga el archivo `Tablero de OEE Industrial.pbix` incluido en este repositorio.
2. Ábrelo con Power BI Desktop.
3. Navega por las diferentes pestañas (OEE, Paros, Tiempos Medios) y utiliza los botones dinámicos para explorar los datos por Tipo de Maquinaria, Incidentes y Periodos de Tiempo.
