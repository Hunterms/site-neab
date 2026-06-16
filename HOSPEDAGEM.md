# NEAB Unicamp — Hospedagem e tecnologia (pesquisa)

> Pesquisa feita inspecionando os sites da própria família COCEN e o catálogo da
> DeTIC/CCUEC (Diretoria de TIC da Unicamp), já que a resposta do NEAB estava demorando.

## O que a família COCEN usa (evidência técnica)
Inspeção de headers HTTP e sinais de CMS dos núcleos:

| Núcleo | Tecnologia | Tema |
|---|---|---|
| PAGU, NEPA, NIPE | WordPress (Unicamp) | **`bx-unicamp-multisite`** (tema padrão Unicamp) |
| NEPO | WordPress | The7 (tema próprio) |
| NIED | WordPress | nied-theme-2023 (tema próprio) |
| NEPAM | WordPress | ColorMag Pro (tema próprio) |
| COCEN (portal) | PHP custom (openresty) | — |
| CMU, CESOP | sites mais antigos/custom | — |

**Conclusão:** o padrão de fato é **WordPress** com subdomínio `nome.unicamp.br`.
Núcleos novos (PAGU/NEPA/NIPE) estão no **tema multisite oficial**; os mais antigos
rodam WordPress próprio com tema custom.

## O serviço oficial: "Websites para todos" (DeTIC)
Fonte: catálogo DeTIC (detic.unicamp.br/catalogo-servicos/websites-para-todos).
- Solução de site institucional pra **órgãos, centros e NÚCLEOS** da Unicamp.
- **É WordPress, com tema padronizado.** ⚠️ **Não é permitido instalar tema próprio**
  ("as necessidades do tema devem ser tratadas de forma colaborativa").
- Pré-requisito: **subdomínio `.unicamp.br` registrado** (via administrador de rede do
  órgão → CCUEC/DeTIC, regulado pela IN ConTIC-IN-01/2019).
- Precisa de um **docente ou funcionário como administrador** (a coordenação do NEAB).
- Solicitação por **portal de chamados** (criar site, publicar, novas features,
  problemas, gestão de usuários). Suporte seg–sex 9h–17h, resposta em até 1 dia útil.
- CMS amigável nativo → atende o requisito de manutenção por equipe não-técnica.

Também existe **Hospedagem Web** do CCUEC (hospedar páginas na infra da Unicamp, com
usuário institucional, Decisão ConTIC D-18/2011) — caminho pra site próprio/estático.

## As 3 rotas possíveis pro NEAB

### A) "Websites para todos" — WordPress gerenciado (tema padrão)
- ✅ Mais fácil, suportado pela DeTIC, grátis, `neab.unicamp.br`, CMS amigável.
- ✅ É o que os núcleos novos usam (PAGU/NEPA/NIPE).
- ❌ **Tema padronizado** — nosso design custom NÃO entra como está; daria pra
  aproximar via customização colaborativa, mas fica com "cara de Unicamp padrão".

### B) WordPress próprio com tema custom (como NEPO/NIED)
- ✅ **Liberdade total de design** — a gente converte nosso mockup num **tema WordPress**.
- ✅ CMS amigável (WordPress) + `neab.unicamp.br`.
- ❌ Precisa de hospedagem que permita tema próprio (CCUEC Hospedagem Web ou servidor
   do COCEN) e de alguém pra montar/manter o WP. Menos "gerenciado".

### C) Site estático (nosso HTML) na Hospedagem Web do CCUEC
- ✅ Nosso design **exatamente como está**, leve e rápido.
- ❌ **Sem CMS** → equipe não-técnica não edita (falha o requisito) — a não ser que a
   gente acople um CMS git-based/headless (complica).

## Recomendação
1. **Primeiro passo (vale pra qualquer rota):** registrar o subdomínio **`neab.unicamp.br`**
   via o administrador de rede do COCEN / DeTIC.
2. **Decisão central — fidelidade de design × serviço gerenciado:**
   - Se o objetivo é facilidade + suporte oficial → **Rota A** (WordPress "Websites para
     todos"), e usamos nosso mockup como referência pra aproximar o tema padrão.
   - Se o diferencial visual afrocentrado importa (nossa tese desde o início) → **Rota B**
     (tema WordPress custom feito do nosso design). É o caminho dos núcleos que quiseram
     identidade própria (NEPO/NIED).
3. **Perguntar à DeTIC** (chamado) o que é permitido hoje pro NEAB: tema próprio no
   serviço? Hospedagem Web pra WordPress próprio? Isso fecha a decisão A vs B.

## Impacto no que já fizemos
O mockup estático continua valioso em qualquer rota: é o **design de referência** pra
Rota A, o **spec do tema** pra Rota B, ou **deploy direto** na Rota C.
