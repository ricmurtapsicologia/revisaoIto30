# Revisão da ITO 30 — Consulta Técnica à Tropa

Página pública de apoio à consulta técnica da minuta da nova ITO 30 — Atendimento a Tentativas de Suicídio — Sistema ATTS.

## Objetivo

Centralizar em uma única experiência:

- acesso à minuta em revisão;
- preenchimento da contribuição técnica diretamente na própria página;
- encaminhamento das respostas ao Google Forms apenas como backend de armazenamento.

O respondente não precisa abrir ou acessar visualmente o Google Forms.

## Página

`https://ricmurtapsicologia.github.io/revisaoIto30/`

## Minuta

`https://docs.google.com/document/d/11RH0jaZOul9qNh7hrTRLXc-DClndHEFW/edit?usp=drive_link&ouid=108383429800204795084&rtpof=true&sd=true`

## Integração com Google Forms

O formulário HTML da página envia os dados diretamente ao endpoint `formResponse` do Google Forms. O Forms funciona somente como backend de coleta.

Mapeamento atual:

- Nome completo → `entry.2051715658`
- Posto/Graduação → `entry.1776044509`
- Melhor e-mail → `entry.2085063746`
- Parte da ITO → `entry.1314340447`
- Fragmento atual → `entry.435462653`
- Justificativa → `entry.1714859578`
- Nova proposta → `entry.1328219941`
- Referência opcional → `entry.1240379903`

Se a estrutura das perguntas do Google Forms for alterada ou recriada, conferir os IDs `entry.*` antes de publicar nova versão da página.

## UX

Fluxo principal:

1. acessar a minuta;
2. preencher a contribuição diretamente na página;
3. enviar;
4. receber confirmação sem sair do site;
5. optar por enviar outra sugestão, mantendo os dados de identificação já preenchidos.

Cada envio corresponde preferencialmente a uma sugestão.

## Estrutura

- `index.html` — página completa, responsiva, formulário integrado e JavaScript de envio;
- `.nojekyll` — impede processamento desnecessário pelo Jekyll.

## Identidade visual

O hero segue a linguagem visual da página CATS Pouso Alegre, adaptada para a Comissão de Revisão da ITO 30, sem os dados do curso.
