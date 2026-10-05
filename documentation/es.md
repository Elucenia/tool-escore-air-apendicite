<!-- ELUCENIA technical documentation · escore-air-apendicite · es · no clinical/professional/rights approval -->

# Puntuación AIR (respuesta inflamatoria en la apendicitis)

[condiciones, fuentes y permisos](https://elucenia.org/es/herramientas/escore-air-apendicite)

## Cómo usar

Utilice la herramienta en el portal o abra index.html mediante un servidor HTTP local. Seleccione el idioma, complete los campos y calcule.

## Entradas y unidades

### Vómitos

`vomito`

### Dolor en la fosa ilíaca derecha

`dor`

### Dolor a la descompresión o defensa muscular

`defesa`

- `0` — Ausente
- `1` — Leve
- `2` — Moderada
- `3` — Intensa

### Temperatura ≥ 38,5 °C

`temp`

### Neutrófilos

`neut`

- `0` — \< 70%
- `1` — 70 a 84%
- `2` — ≥ 85%

### Leucocitos

`leuco`

- `0` — \< 10.000/mm³
- `1` — 10.000 a 14.900/mm³
- `2` — ≥ 15.000/mm³

### Proteína C reactiva

`pcr`

- `0` — \< 10 mg/L
- `1` — 10 a 49 mg/L
- `2` — ≥ 50 mg/L

## Edición del método

AIR de Andersson (2008), con las Tablas 2 y 7 corregidas por la fe de erratas de 2012: siete componentes, total 0–12, PCR en mg/L; grupos originales 0–4, 5–8 y 9–12. No se ha aplicado el cambio del punto de corte inferior propuesto en 2021.

## Fórmula documentada

Vómitos (1) + dolor en fosa ilíaca derecha (1) + irritación peritoneal leve (1), moderada (2) o intensa (3) + temperatura ≥38,5 °C (1) + neutrófilos 70–84% (1) o ≥85% (2) + leucocitos 10.000–14.900 (1) o ≥15.000 (2) + PCR 10–49 (1) o ≥50 mg/L (2). Total 0 a 12.

## Límites y población

El AIR de 2008 se estudió en personas ingresadas por sospecha de apendicitis; parte de la cohorte permaneció en el grupo indeterminado y necesitó más investigación. Del artículo original de 2008 solo se leyó el resumen. La fe de erratas de 2012 se leyó directamente: sus Tablas 2 y 7 corrigen las concentraciones de PCR y documentan los puntos, las unidades y los grupos originales. La comprobación numérica se limita a sumar los siete componentes ya seleccionados; no aprueba los grupos clínicos ni las decisiones diagnósticas, de imagen o quirúrgicas. La revisión de 2021 propuso riesgo bajo con una puntuación \<4, distinto del grupo original 0–4; ese cambio no se ha aplicado en esta edición. La edad mínima, las exclusiones y el protocolo completo no se confirmaron mediante la lectura del resumen de 2008. Los hallazgos no observados no deben considerarse ausentes. No se han realizado una revisión clínica ni lingüística por profesionales independientes ni una autorización de los derechos del instrumento.

## Referencias

- [Andersson M, Andersson RE. The appendicitis inflammatory response score: a tool for the diagnosis of acute appendicitis that outperforms the Alvarado score. World J Surg, 2008.](https://doi.org/10.1007/s00268-008-9649-y)

- [Di Saverio S et al. Diagnosis and treatment of acute appendicitis: 2020 update of the WSES Jerusalem guidelines. World J Emerg Surg, 2020.](https://doi.org/10.1186/s13017-020-00306-3)

- [Andersson M, Andersson RE. Erratum to: The Appendicitis Inflammatory Response Score: A Tool for the Diagnosis of Acute Appendicitis that Outperforms the Alvarado Score. World J Surg, 2012;36:2269–2270. Corrected Tables 2 and 7.](https://doi.org/10.1007/s00268-012-1679-9)

## Reproducir las pruebas técnicas

Ejecute node test.cjs en el directorio raíz de este repositorio para repetir los casos sintéticos registrados. Se conservan las entradas, los resultados esperados y las tolerancias originales. Las pruebas técnicas no constituyen validación clínica.

```sh
node test.cjs
```

tool.json contiene las fuentes, la edición y el alcance de la revisión. examples.json conserva las entradas y los resultados esperados de los casos sintéticos; results.json registra los resultados obtenidos.

[Ficha y referencias](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referencia](../examples.json) · [results.json](../results.json)

## Revisión y condiciones de uso

No se ha realizado una revisión clínica independiente.

Esta interfaz es una traducción de elaboración propia, no una edición oficial o certificada. No se han realizado la revisión clínica independiente, la revisión lingüística profesional ni la autorización de derechos de los instrumentos.

Resultado de la fórmula o clasificación. La interpretación, la conducta y la aplicabilidad dependen de la evaluación profesional y de la fuente seleccionada.

## Licencia y atribución

Apache-2.0 se aplica únicamente al código de ELUCENIA. Los derechos de los instrumentos, publicaciones, traducciones y datos permanecen en manos de sus respectivos titulares. Conserve LICENSE y NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
