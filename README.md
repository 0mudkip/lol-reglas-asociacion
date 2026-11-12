# Reglas de asociación en drafts de League of Legends

Proyecto de Minería de Datos. Aplica análisis de canasta (Apriori y FP-Growth) a 42,498 partidas de SoloQ de
LAN: cada equipo es una transacción y sus 5 campeones son los artículos.

- `reglas_asociacion_lol.ipynb`: el análisis completo, con resultados y gráficas.
- `PENDIENTES.md`: cambios que quedan por hacer.
- `requirements.txt`: librerías necesarias.

## Cómo correrlo

1. Instala las librerías: `pip install -r requirements.txt`.
2. Copia el archivo de partidas a `datos/todas.jsonl`. No se versiona; se genera con el extractor del proyecto
   [lol-draft-predictor](https://github.com/0mudkip/lol-draft-predictor) (`ml/datos/todas.jsonl`).
3. Abre el notebook y corre las celdas en orden.
