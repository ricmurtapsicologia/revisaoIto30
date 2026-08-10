# Revisão da ITO 30 — Consulta Técnica à Tropa

Página pública de apoio à consulta técnica da minuta da nova ITO 30 — Atendimento a Tentativas de Suicídio — Sistema ATTS.

## Experiência do usuário

A página é mobile-first e concentra leitura e contribuição em um único endereço.

- **Visualizar minuta**: abre a minuta em leitor próprio baseado em PDF.js, sem Google Drive/Docs visível ao usuário.
- O leitor inicia ajustado à largura, renderiza páginas progressivamente e preserva a paginação oficial do PDF.
- Há navegação anterior/próxima, indicação de página, busca textual e zoom no desktop.
- O botão **Sugerir alteração desta página** abre o formulário e registra automaticamente o número da página no campo do fragmento.
- **Responder**: revela o formulário somente quando solicitado.
- O Google Forms permanece apenas como backend de armazenamento das respostas.
- Após o envio, a página permite registrar nova contribuição ou retornar à página da minuta em que o usuário estava.

## Endereço

`https://ricmurtapsicologia.github.io/revisaoIto30/`

## Minuta

O leitor utiliza o arquivo local:

`minuta-ito30.pdf`

O PDF é sincronizado para o repositório pelo workflow:

`.github/workflows/sync-minuta.yml`

Fonte oficial atual — ITO 30 V3.3:

`https://drive.google.com/file/d/1f0m-Vvg-RupgOkvpwmBI_zDHOkC07iQU/view?usp=drive_link`

A opção por manter uma cópia local no GitHub Pages evita expor a interface do Google Drive ao avaliador e melhora a estabilidade do leitor PDF.js.

## Leitor PDF

Biblioteca utilizada:

- PDF.js `4.10.38`
- carregamento da biblioteca via jsDelivr;
- PDF hospedado no próprio GitHub Pages;
- renderização progressiva/lazy por página;
- renderização considerando densidade da tela para melhorar nitidez;
- busca textual feita somente quando solicitada.

## Google Forms — backend

As respostas são enviadas silenciosamente para:

`https://docs.google.com/forms/d/e/1FAIpQLSehw1svEtR132gzqSuQM54D45IuOyeN2BZtaeDiRsRgVeEioQ/formResponse`

IDs integrados atualmente:

- Nome: `entry.2051715658`
- Posto/Graduação: `entry.1776044509`
- E-mail: `entry.2085063746`
- Parte da ITO: `entry.1314340447`
- Fragmento: `entry.435462653`
- Justificativa: `entry.1714859578`
- Nova proposta: `entry.1328219941`
- Referência: `entry.1240379903`

Se o Google Forms for recriado ou suas perguntas forem substituídas, esses IDs deverão ser conferidos.

## Arquivos principais

- `index.html` — página completa, leitor PDF.js e formulário integrado.
- `minuta-ito30.pdf` — PDF oficial apresentado no leitor.
- `.github/workflows/sync-minuta.yml` — sincronização do PDF oficial a partir do Google Drive.
- `.nojekyll` — publicação estática sem processamento Jekyll.

## Identidade visual

O hero segue a linguagem visual da página CATS Pouso Alegre, adaptada à Comissão de Revisão da ITO 30.

Assinatura institucional apresentada na página:

**Richelmy Murta, Major BM**  
Presidente da Comissão de Revisão da ITO 30
