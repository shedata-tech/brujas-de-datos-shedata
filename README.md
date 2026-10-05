# 🔮 Brujas de Datos: La Apertura

**She Data · Charla 1** — con **Lina Serna** ✨

📅 Sábado 3 de octubre de 2026 · 3:00 PM (COL)
🪄 Fundadora de la comunidad She Data

Hola, hermosa. Bienvenida al primer encuentro de **Brujas de Datos** — hoy no hablamos de teoría, abrimos un dataset real y vemos, paso a paso, cómo trabajamos los datos en She Data: de la curiosidad al insight.

## 🧹 El dataset

Los **152 juicios de brujería de Salem (1692)**, compilados por el historiador Richard Latner (Tulane University). Sí, leíste bien: investigamos a las *brujas originales* con las herramientas de las *brujas de datos* de hoy.

Archivo: [`brujas_acusadas_salem_1692.csv`](brujas_acusadas_salem_1692.csv)

| Columna | Descripción |
|---|---|
| `nombre` | persona acusada formalmente de brujería |
| `residencia` | pueblo donde vivía al momento de la acusación |
| `mes_acusacion` | mes de 1692 en que fue acusada |
| `mes_ejecucion` | mes en que fue ejecutada (vacío si no lo fue) |
| `ejecutada` | Sí / No |

## 📓 El notebook

[`BrujasDatos.ipynb`](BrujasDatos.ipynb) recorre el análisis completo:

1. **Cargar los datos** — mirar los datos crudos antes de asumir nada.
2. **Limpieza rápida** — nulos, tipos y valores raros antes de confiar en nada.
3. **Las preguntas que le hacemos a los datos** — de dónde eran las acusadas, cuándo se disparó la histeria, qué proporción terminó ejecutada.
4. **Cruzando variables** — lugar + tiempo, para ver el patrón de propagación.
5. **Cierre con magia** — ¿se podía predecir quién sería acusada?

## 🚀 Cómo correrlo

**Google Colab (recomendado):**
Sube `BrujasDatos.ipynb` y `brujas_acusadas_salem_1692.csv` a la misma sesión (o móntalos desde Drive).

**Local:**
```bash
pip install pandas matplotlib
jupyter notebook BrujasDatos.ipynb
```

El notebook lee el CSV con ruta relativa (`pd.read_csv("brujas_acusadas_salem_1692.csv")`), así que mantén ambos archivos en la misma carpeta.

---

Creado con 💗 por la comunidad **She Data** — *ninguna mujer aprende datos sola* ✨
