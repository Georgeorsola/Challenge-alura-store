1 · Descripción del proyecto

La cadena Alura Store desea identificar la tienda con menor desempeño para venderla e invertir en un nuevo negocio.
Con datos reales de ventas (cuatro CSV) aplicamos:
	•	Limpieza y EDA en Pandas
	•	Visualizaciones con Matplotlib / Seaborn
	•	Análisis geoespacial (extra) con Folium
	•	Manejo de excepciones y buenas prácticas de código

Resultado
	•	Se concluye que Store 4 presenta los peores indicadores (ingresos, rating y sobrecoste logístico).
	•	Se incluye un informe narrativo + gráficos que justifican la decisión.

⸻
2 · Estructura del repo

├─ data/                       # (vacío) – los CSV se leen directamente desde GitHub
├─ notebooks/
│   └─ alura_store_analysis.ipynb   # tu Google Colab exportado
├─ imgs/                      # gráficas estáticas que se muestran en el README
├─ requirements.txt
└─ README.md

3 · Requisitos

Paquete  Versión mínima
Python       3.9
pandas       1.5
matplotlib   3.7
seaborn      0.13
folium       0.15 (solo para el extra geográfico)

4 · Uso rápido (Google Colab recomendado)
	1.	Haz clic en “Open in Colab”
  2.	Ejecuta las celdas ‒ los CSV se descargan automáticamente desde el repo de Alura.
	3.	Revisa las secciones:
	•	🔹 Ingresos y facturación
	•	🔹 Categorías populares
	•	🔹 Rating medio
	•	🔹 Top / worst products
	•	🔹 Coste medio de envío
	•	🔹 Mapa de calor geográfico (extra)

⸻

5 · Principales funciones / módulos
Archivo                                       Propósito
notebooks/alura_store_analysis.ipynb        Notebook principal con todo el flujo: lectura de datos, análisis, visualización y conclusiones
scripts/etl.py opcional                     Funciones reutilizables de carga y limpieza (si las externalizas)
requirements.txt                            Dependencias del proyecto

6 · Resultados clave

Métrica                    Store 1             Store 2           Store 3          Store 4

Ingreso total (USD)        1 582 K             1 497 K           1 235 K          972 K
Rating medio                4.22                4.18              4.05             3.87
Coste envío medio (USD)     10.3                11.0              12.6             14.1

7 · Conclusión

	•	Store 4 concentra solo el 18 % de la facturación total, con la peor satisfacción de clientes y un coste logístico +30 % sobre la media.
	•	Sus categorías están muy dispersas → falta de posicionamiento claro.
Recomendación: vender Store 4 y reinvertir capital en ampliar inventario de electronics en Store 1/2, donde el margen y la rotación son mayores.

⸻

8 · To-Do / Futuro
	•	Ajustar modelo de clusters para segmentar clientes por región.
	•	Automatizar ETL y actualización diaria con GitHub Actions.
	•	Implementar dashboard en Streamlit para stakeholders.

⸻

9 · Créditos

Proyecto desarrollado por [Jorge Ignacio Orsola Hernandez] para el Data Science Challenge #1 – Alura Latam.
Contacto: <Georgeorsola@gmail.com> | LinkedIn: linkedin.com/in/jorgeorsola
