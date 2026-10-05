<!-- ELUCENIA technical documentation · escore-air-apendicite · pt-BR · no clinical/professional/rights approval -->

# Escore AIR (Appendicitis Inflammatory Response)

[condições, fontes e permissões](https://elucenia.org/pt-br/ferramentas/escore-air-apendicite)

## Como usar

Use a ferramenta no portal ou abra index.html em um servidor HTTP local. Selecione o idioma, preencha os campos e calcule.

## Entradas e unidades

### Vômitos

`vomito`

### Dor na fossa ilíaca direita

`dor`

### Descompressão dolorosa ou defesa muscular

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

### Leucócitos

`leuco`

- `0` — \< 10.000/mm³
- `1` — 10.000 a 14.900/mm³
- `2` — ≥ 15.000/mm³

### Proteína C reativa

`pcr`

- `0` — \< 10 mg/L
- `1` — 10 a 49 mg/L
- `2` — ≥ 50 mg/L

## Edição do método

AIR de Andersson (2008), com as Tabelas 2 e 7 corrigidas pela errata de 2012: sete componentes, total 0–12, PCR em mg/L; grupos originais 0–4, 5–8 e 9–12. A mudança do corte inferior proposta em 2021 não foi aplicada.

## Fórmula documentada

Vômitos (1) + dor na fossa ilíaca direita (1) + irritação peritoneal leve (1), moderada (2) ou intensa (3) + temperatura ≥ 38,5 °C (1) + neutrófilos 70–84% (1) ou ≥ 85% (2) + leucócitos 10.000–14.900 (1) ou ≥ 15.000 (2) + PCR 10–49 (1) ou ≥ 50 mg/L (2). Total de 0 a 12.

## Limites e população

O AIR de 2008 foi estudado em pessoas admitidas por suspeita de apendicite; parte da coorte permaneceu em faixa indeterminada e necessitou investigação adicional. O artigo original de 2008 foi lido somente pelo resumo. A errata de 2012 foi lida diretamente: suas Tabelas 2 e 7 corrigem as concentrações de PCR e documentam os pontos, as unidades e os grupos originais. A conferência numérica limita-se à soma dos sete componentes já selecionados; não aprova os grupos clínicos nem decisões de diagnóstico, imagem ou cirurgia. A revisão de 2021 propôs baixo risco com escore \<4, distinto do grupo original 0–4; essa mudança não foi aplicada nesta edição. Idade mínima, exclusões e protocolo completo não foram confirmados pela leitura do resumo de 2008. Achados não observados não devem ser tratados como ausentes. Revisão clínica e de idiomas por profissionais independentes e autorização de direitos do instrumento não realizadas.

## Referências

- [Andersson M, Andersson RE. The appendicitis inflammatory response score: a tool for the diagnosis of acute appendicitis that outperforms the Alvarado score. World J Surg, 2008.](https://doi.org/10.1007/s00268-008-9649-y)

- [Di Saverio S et al. Diagnosis and treatment of acute appendicitis: 2020 update of the WSES Jerusalem guidelines. World J Emerg Surg, 2020.](https://doi.org/10.1186/s13017-020-00306-3)

- [Andersson M, Andersson RE. Erratum to: The Appendicitis Inflammatory Response Score: A Tool for the Diagnosis of Acute Appendicitis that Outperforms the Alvarado Score. World J Surg, 2012;36:2269–2270. Corrected Tables 2 and 7.](https://doi.org/10.1007/s00268-012-1679-9)

## Reproduzir os testes técnicos

Execute node test.cjs na pasta raiz deste repositório para repetir os casos sintéticos registrados. As entradas, expectativas e tolerâncias originais são preservadas. Testes técnicos não constituem validação clínica.

```sh
node test.cjs
```

tool.json contém fontes, edição e escopo de revisão. examples.json conserva as entradas e expectativas sintéticas; results.json registra os resultados obtidos.

[Ficha e referências](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referência](../examples.json) · [results.json](../results.json)

## Revisão e condições de uso

Revisão clínica independente não realizada.

Esta interface é uma tradução autoral, não uma edição oficial ou certificada. Revisão clínica independente, revisão linguística profissional e autorização de direitos de instrumentos não foram realizadas.

Resultado da fórmula ou classificação. Interpretação, conduta e aplicabilidade dependem da avaliação profissional e da fonte selecionada.

## Licença e atribuição

Apache-2.0 aplica-se somente ao código da ELUCENIA. Os instrumentos, publicações, traduções e dados mantêm os direitos dos respectivos titulares. Preserve LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
