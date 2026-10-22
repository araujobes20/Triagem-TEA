# Triagem TEA

Questionário web (HTML, CSS e JavaScript, sem dependências) que gera um relatório de triagem para Transtorno do Espectro Autista: sinais compatíveis, nível de suporte estimado, perfil de apresentação e possíveis condições associadas.

> **Ferramenta de triagem e apoio educacional. Não diagnostica.** O diagnóstico exige avaliação clínica com instrumentos como ADOS-2 e ADI-R. Todo o processamento ocorre no navegador, sem envio de dados.

## Como publicar no GitHub Pages

1. Crie um repositório e envie `index.html` e este `README.md`.
2. Em **Settings → Pages**, escolha **Deploy from a branch**, branch `main`, pasta `/ (root)`.
3. O app ficará em `https://SEU-USUARIO.github.io/NOME-DO-REPO/`.

## Base científica

Yu, Y., Ozonoff, S., & Miller, M. (2024). *Assessment of Autism Spectrum Disorder*. Assessment, 31(1), 24–41. doi:10.1177/10731911231173089

## Lógica de pontuação

Itens pontuados de 0 a 3. Cada componente diagnóstico tem 2 itens (soma de 0 a 6) e conta como presente com soma ≥ 4.

| Elemento | Regra |
|---|---|
| Critério A (DSM-5-TR) | Os 3 componentes presentes: reciprocidade socioemocional, comunicação não verbal, relacionamentos |
| Critério B | Pelo menos 2 de 4: movimentos/fala repetitivos, rotinas, interesses restritos, sensorial |
| Critério C | Itens de início precoce com pontuação ≥ 2 |
| Critério D | Item de prejuízo funcional ≥ 2 |
| Nível 1 a 3 | Pelo maior valor entre apoio em comunicação social e apoio por comportamentos repetitivos (0–1 → nível 1, 2 → nível 2, 3 → nível 3) |
| Perfil | Predomínio de domínio (diferença ≥ 15 pontos percentuais), linguagem, deficiência intelectual, sensorial |
| Comorbidades | Ansiedade, TDAH, depressão (3 itens cada; ≥ 4 sinais presentes, ≥ 7 marcantes) e deficiência intelectual (itens cognitivo, adaptativo e linguagem) |

Os pontos de corte são **heurísticos**, derivados dos critérios do DSM-5-TR, e não foram validados psicometricamente. Antes de uso clínico ou de pesquisa, é necessário um estudo de validação (sensibilidade, especificidade, VPP) contra ADOS-2/ADI-R.

## Pontos de atenção

- O DSM-5 unificou autismo, Asperger e TGD-SOE. O relatório mostra a correspondência histórica apenas como informação.
- Itens de camuflagem sinalizam possível subestimação, descrita em mulheres e adultos.
- Resposta positiva ao item de pensamentos de morte ou autolesão exibe orientação imediata (CVV 188, SAMU 192).

## Próximos passos sugeridos

- Registrar respostas anonimizadas para validação (por exemplo, Google Apps Script + Google Sheets, com consentimento e aprovação de comitê de ética).
- Adicionar versões validadas em português (M-CHAT-R/F, SCQ) quando licenciadas.
- Escolher uma licença antes de tornar o repositório público.
