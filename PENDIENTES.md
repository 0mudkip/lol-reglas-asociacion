# Pendientes · Reglas de asociación en drafts de LoL

Estado al 12 de noviembre de 2026: `reglas_asociacion_lol.ipynb` está completo y corre de principio a fin.
Lo que sigue son cambios que se dejaron para después.

## Antes de entregar

- [ ] **Revisar contra la rúbrica del profesor.** El notebook se armó sin las instrucciones de la materia;
      hay que confirmar formato, secciones obligatorias y si pide un algoritmo o métrica en particular.
- [ ] **Datos del encabezado.** Confirmar nombre de la materia, grupo, fecha y si el trabajo es individual o
      en equipo (primera celda del notebook).
- [ ] **Leer y ajustar las conclusiones** (sección 12) con tus propias palabras y tu conocimiento del juego.
- [ ] **Decidir cómo se entregan los datos.** `datos/todas.jsonl` pesa 32 MB; si no se puede subir, entregar
      una muestra o una liga.

## Mejoras al análisis

- [ ] **Agregar baneos como artículos** (`ban_X`): los datos ya traen los baneos por equipo y no se usaron.
- [ ] **Comparar por parche** (16.19, 16.20 y 16.21) igual que se hizo por rango, para ver si las reglas
      cambian con el meta.
- [ ] **Asociaciones negativas:** tabla de pares con lift menor a 1 fuera de la línea inferior (hoy solo se
      ven en el mapa de calor ADC-SUP).
- [ ] **Más métricas de interés:** leverage, convicción y métrica de Zhang (`mlxtend` ya las calcula; solo
      falta mostrarlas y explicarlas).
- [ ] **Corregir por comparaciones múltiples** en el análisis de victoria (Bonferroni o FDR) en lugar de la
      regla práctica de |z| > 3.
- [ ] **Validar las reglas en el tiempo:** minar con los parches 16.19 y 16.20 y comprobar si el lift se
      mantiene en el 16.21.
- [ ] **Recomendador que combine lift y tasa de victoria**, y que respete el rol que falta en el equipo
      (usar las reglas campeón_rol del análisis B).
- [ ] **Agrupamiento de composiciones** (K-Means o jerárquico) para encontrar arquetipos de equipo, si la
      materia pide una segunda técnica.
- [ ] **Reglas por rol en la victoria:** repetir el análisis C con artículos campeón_rol.

## Más datos (requiere volver a usar la API de Riot)

- [ ] **Objetos comprados por jugador**, para el análisis de canasta clásico sobre builds. El extractor
      actual (`lol-draft-predictor/ml/extraer.py`) no los guarda.
- [ ] **Orden de selección del draft**, para saber qué campeón se eligió en respuesta a cuál.
- [ ] **Indicador de dúo**, para separar parejas elegidas a propósito de las que coinciden al azar.

## Otros entregables

- [ ] Reporte escrito o presentación, si la materia lo pide.
- [ ] Exportar el notebook a HTML o PDF para la entrega.
- [ ] Decidir si esta carpeta se sube a un repositorio de Git.
