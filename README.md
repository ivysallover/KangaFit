# 🦘 KangaFit Analytics Hub

**KangaFit** es la primera y única marca del mundo dedicada exclusivamente al arte de la confección de ropa deportiva premium para canguros de alto rendimiento. Este dashboard interactivo permite visualizar el crecimiento masivo, la segmentación por especies y la eficiencia operativa de la empresa en el mercado australiano.

![Logo KangaFit](KangaFit-2.png)
*Identidad visual de la marca líder en rendimiento marsupial.*

## 🚀 Cómo ejecutar el proyecto
Para visualizar el dashboard correctamente y permitir que el navegador cargue los datos relacionales, es necesario usar un servidor local:

1.  **Instalar Live Server**: Si usas VS Code, busca la extensión "Live Server" e instálala.
2.  **Lanzar el Dashboard**: Abre el archivo `kangafit.html`, haz clic derecho y selecciona **"Open with Live Server"**.
3.  **Acceso**: Se abrirá automáticamente en tu navegador (usualmente en `http://127.0.0.1:5500`).

> **Nota:** Abrir el archivo directamente (`file://...`) puede bloquear la carga del JSON por políticas de seguridad del navegador (CORS).

## 📊 Arquitectura de Datos (Data Engineering)
A diferencia de otros dashboards con datos estáticos, KangaFit utiliza un **motor de simulación probabilística** desarrollado en Python para generar un ecosistema de datos coherente:

* **Fuente de Verdad**: El script genera un archivo `KangaFit.json` con más de **150,000 líneas de código JSON**.
* **Modelo de Negocio (Premium Accessible)**: El generador está calibrado para una marca "Masstige" (Mass-Prestige), simulando un volumen de ventas trimestral de aproximadamente **12,000 unidades** y un revenue de **$1.8M AUD**.
* **Integridad Lógica**: 
    * **Devoluciones**: Vinculadas a motivos específicos por producto (ej. un producto de combate no reporta problemas de "bolsillo marsupial").
    * **Reviews**: Generadas dinámicamente; el texto de la reseña coincide estrictamente con la categoría del producto comprado.
* **Crecimiento S-Logístico**: Las ventas mensuales siguen una curva de crecimiento real, considerando la estacionalidad del *Outback* australiano y la expansión geográfica por regiones (Queensland, Victoria, NSW).

## 🛠️ Tecnologías utilizadas
* **Backend / Data Gen**: Python 3 (librerías `json`, `random`, `math`, `datetime`).
* **Frontend**: HTML5, CSS3 (Custom Properties), JavaScript (ES6+).
* **Visualización**: [Chart.js](https://www.chartjs.org/) para gráficos interactivos con efectos de *spotlight* y filtrado dinámico.
* **Reportes**: Soporte para exportación de métricas a **Excel (CSV)** y generación de auditorías en **PDF**.

## 📈 Insights Clave
* **Efecto Joey**: El análisis de lenguaje natural revela que una gran parte de las reviews menciona necesidades para las crías (*joeys*), identificando una oportunidad de mercado no atendida.
* **Segmento Élite**: El Canguro Rojo se mantiene como el líder de mercado, mientras que el Canguro Arbóreo representa el ticket promedio más alto debido a la especialización técnica requerida.

---
*Este proyecto forma parte de un trabajo final de la catedra de  Visualizacion de Datos de la carrera Ciencia de Datos (UCA Rosario).*
