# NEAB Unicamp — Direção Visual (Fase 2)

> Sistema de design aplicado no mockup da Home ([mockup/index.html](mockup/index.html)).
> Derivado de [IDENTIDADE-VISUAL.md](IDENTIDADE-VISUAL.md). Validado com contraste real
> (AA) e teste responsivo (375 / 1280px).

## ⭐ v3 — direção ATUAL: minimalista + glassmórfica (decisão do user)
O user descartou o hero dark/aurora ("ficou feio") e pediu **minimalismo + glass**,
paleta enxuta e navbar flutuante. Esta é a direção vigente; v1/v2 abaixo são histórico.

- **Paleta enxuta (tokens estilo design-system):** `--bg` creme (#FAF5EC), `--fg`
  (#2A211C), `--muted` (#6B5D52), `--primary` terracota (#9E2B25) + `--primary-fg`
  (#FFF7EF), `--secondary` ocre (#E8A02C) + `--secondary-fg`. Cor usada com parcimônia:
  terracota nos CTAs/tags/1 bloco; ocre só em micro-acentos.
- **Glassmorfismo:** painéis translúcidos (`rgba(255,255,255,.55)` + blur 16px + borda
  clara). Pra o glass "ler", há **blobs de cor bem sutis** (terracota/ocre, ~10% opac.)
  fixos no fundo creme — minimalismo com profundidade (substituiu a aurora dark).
- **Navbar flutuante centralizada (pill glass)** — não ocupa todo o width; dropdowns
  glass. Mobile = sheet glass deslizante. (pedido do user: "mais tech e elegante".)
- **Hero minimal centrado** — título grande, typewriter "Pesquisa que afirma [...]",
  2 botões, pill glass "criado em 2024". Sem fundo pesado.
- **"O que é" = único bloco de cor** (card terracota arredondado). 1 momento de cor forte.
- **Blog cards** (ref. shadcn BlogPostCard): tag pill `primary/10`, título com underline
  que cresce no hover, hover-lift. **Profile cards** (equipe): adaptados do ref. neumórfico
  → versão glass minimal, avatar com iniciais em gradiente, tags, links Lattes/e-mail
  (NÃO "seguir/mensagem"). Footer minimal claro.
- Contraste AA reverificado: `muted/bg` 5.84 · `primary/bg` 6.84 · `primary-fg/primary`
  7.01 · `muted/glass` 6.08 ✓. Eyebrow sobre o card terracota usa `--gold-soft`
  (#F6CE84 = 4.98:1), pois ocre puro reprova (3.36:1).

### v5 — prep pro critique (pedidos do user)
- **Logo real** (`neab.png` — badge circular afro ouro/ocre/preto) substituiu o glifo
  placeholder na navbar, sheet e footer. Removido o círculo de degradê de trás.
- **Sem degradê onde não há foto** → **cor sólida única** (`--primary` terracota) em
  todos os placeholders: miniaturas de notícia e avatares da equipe.
- **Fotos afro reais no hero** (exemplos do **Wikimedia Commons**, livres): samba de roda,
  capoeira, maracatu, candomblé, saias coloridas. **Cor original, sem efeito** (removido o
  duotone/multiply e o filtro). 8 tiles desktop (parallax) + 4 no fundo mobile (cor cheia,
  legibilidade pelo scrim). Pasta `mockup/img/` (h1–h9; usadas h1,h2,h3,h4,h6,h8).
  → Trocar pelas fotos do próprio NEAB quando vierem.

### Ajustes v4 (pedidos do user)
- **Navbar voltou a full-width** (sticky, glass sutil, borda inferior) — "mais formal".
  Mantém dropdowns glass e sheet mobile.
- **Áreas de atuação = Spotlight cards** (ref. shadcn SpotlightCard): cards escuros
  (`--espresso2` #241712), brilho radial que segue o mouse — **recolorido pro ocre/
  laranja** (não o roxo original). Vira uma faixa de contraste tech.
- **Hero com imagens flutuantes (parallax)** (ref. Floating/motion): tiles de imagem
  que driftam com o mouse em profundidades diferentes, atrás de um scrim que mantém o
  texto legível. ⚠️ Imagens são **placeholders em duotone terracota** (picsum grayscale +
  multiply); trocar pelas fotos reais do NEAB (eventos/pessoas). Ocultas no mobile.
- Imagens são prioridade do NEAB → este hero é o lugar natural pra elas brilharem.
- **+ fotos no hero** (10 tiles no desktop) e **fundo de fotos no mobile** (container
  `.floating-m`, 4 tiles estáticos ~42% atrás de scrim reforçado).
- **Pesquisa & Extensão = BorderRotate** (ref. do user): card escuro (`--espresso2`) com
  **borda em gradiente cônico dourado girando** (via `@property --ga` + keyframes, 6s).
  Pareia com os spotlight cards das áreas → dois "momentos escuros" coerentes. Para com
  `prefers-reduced-motion`.

---
### Histórico (v1 clara, v2 dark/aurora) — substituídas pela v3

## Tipografia
- **Títulos:** Fraunces (serif quente, editorial, com caráter). Usa itálico pra
  destacar termos ("Afro-Brasileiros").
- **Corpo:** Inter (sans limpa, alta legibilidade).
- Decisão: confirma a direção "serif de caráter + sans legível" do briefing.

## Paleta (com contraste verificado — WCAG AA)
| Token | Hex | Contraste medido | Uso |
|---|---|---|---|
| Tinta (texto) | `#2A211C` | 13.7:1 no creme ✓ | corpo, títulos escuros |
| Tinta suave | `#5A4D44` | 7.07:1 no creme ✓ | texto secundário |
| Terracota | `#9E2B25` | 6.46:1 no creme ✓ | cor âncora, títulos, botões |
| Branco quente | `#FFFDF8` | 7.31:1 no terracota ✓ | texto sobre terracota, cards |
| Ocre | `#E8A02C` | 7.12:1 no tinta ✓ | acento em fundo escuro (datas) |
| **Ocre claro** | `#F6CE84` | 4.98:1 no terracota ✓ | **texto pequeno sobre terracota** |
| Creme | `#F7EEDF` | — | fundo quente padrão |
| Verde / Magenta | `#2E7D32` / `#D6447D` | — | acentos pan-africanos, gradiente |

⚠️ **Regra de ouro:** o `--ocre` (#E8A02C) NÃO passa AA como texto pequeno sobre
terracota (3.36:1). Pra texto pequeno sobre terracota, usar `--ocre-claro` (#F6CE84).
Ocre normal só em fundo escuro ou peças grandes/decorativas.

## Gradiente assinatura
`linear-gradient(120deg, #E8A02C → #E2682A → #D6447D)` — vem do logo. Usado no badge,
no bloco do hero e em miniaturas de notícia.

## Grafismos
- Glifo geométrico afro (estilo adinkra) em SVG — usado no badge do logo, hero e como
  marca d'água sutil (10% opacidade) na faixa terracota.
- Faixa pan-africana (terracota/ocre/verde) como divisória no rodapé do hero.
- ⚠️ **O glifo atual é PLACEHOLDER** (recriado à mão). Substituir pelo logo oficial
  do NEAB quando tivermos o arquivo. Hoje parece um "alvo/mira"; o real é um símbolo
  adinkra próprio.

## Atualização v2 (refs trazidas pelo user: shadcn navbar, aurora, typewriter)
- **Navbar com mega-dropdowns** (estilo shadcn NavigationMenu): O Núcleo / Pesquisa /
  Acervo abrem painel com ícones + título + descrição. Atividades e Notícias = links
  simples. Contato = botão. Mobile vira **sheet** (slide da direita) com acordeões.
- **Hero escuro + "aurora"** — a técnica de glows radiais nos cantos do "Aurora Dream
  Corner Whispers", mas **recolorida na paleta NEAB** (ocre, laranja, magenta, terracota
  sobre base espresso). ⚠️ Descartada a paleta original (lavanda/rosa/azul pastel) por
  brigar com a identidade afrocentrada.
- **Typewriter** (JS vanilla) na linha "Pesquisa que afirma [ancestralidade · identidade ·
  memória · futuro · justiça]". Respeita `prefers-reduced-motion` (mostra estática).
- Hero pronto pra receber **foto de fundo** real (hoje: aurora + grão + marca d'água).
- Esses componentes vêm do ecossistema **shadcn/React** → reforça Next.js + shadcn/ui
  como candidato de stack na Fase 3.

## Componentes no mockup
- Header sticky com blur, nav com dropdowns (Contato como botão), sheet no mobile.
- Hero escuro full-bleed: aurora quente + typewriter + faixa pan-africana embaixo.
- Faixa "O que é o NEAB" (terracota, texto branco) — cartão de existência.
- Grid de Áreas de Atuação (6 cards, ícones de linha SVG, hover sutil).
- Destaques: lista de Notícias (miniaturas em gradiente) + painel escuro de Eventos
  (datas em ocre).
- CTA de Pesquisa (card com borda ocre à esquerda).
- Footer escuro, 4 colunas + selos Unicamp/COCEN + link de acessibilidade.

## Acessibilidade aplicada
- Skip link "Pular para o conteúdo".
- Contrastes AA verificados (tabela acima).
- `prefers-reduced-motion` respeitado.
- Foco/teclado, alt/aria nos ícones, viewport meta, fontes ≥16px no corpo.
- Responsivo testado: 375px (mobile, hambúrguer) e 1280px (desktop), sem overflow.

## Pendências
- [ ] Logo oficial do NEAB (substituir o glifo placeholder).
- [ ] Arquivos da identidade pra refinar a paleta (hex exatos).
- [ ] Fotografia real (pessoas, eventos) — hoje há blocos de gradiente no lugar.
- [ ] Validar a direção com a coordenação do NEAB antes de codar o site real.
