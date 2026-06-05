# NEAB Unicamp — Documento de Conhecimento (Fase 1)

> Construído antes de desenhar/codar. Base pra decidir arquitetura e design.

## 1. O ecossistema: COCEN

A **COCEN** (Coordenadoria de Centros e Núcleos Interdisciplinares de Pesquisa) coordena
**23 Centros e Núcleos** da Unicamp, criados desde 1977. São órgãos de pesquisa
científica e tecnológica com abordagem interdisciplinar — cobrem áreas que os
departamentos convencionais não atendem bem.

Estrutura institucional do site da COCEN (menu): Institucional · Centros e Núcleos ·
Pesquisadores · Hubs · Cai-Consu · Bibliotecas · Legislação · Comunicação.

Cada núcleo tem uma **página-padrão dentro do COCEN** (contato, coordenação, equipe,
notícias) e, quando maduro, um **site próprio externo** (ex.: pagu.unicamp.br,
nepo.unicamp.br).

## 2. O NEAB — onde está hoje

**Núcleo de Estudos Afro-Brasileiros**

- **Criado em 26/03/2024** (Deliberação CONSU-A-007/2024) — é o núcleo **mais novo**
  do COCEN (~2 anos). ID 23 na listagem.
- **Missão:** pesquisas interdisciplinares sobre a população afro-brasileira, relações
  étnico-raciais e ações afirmativas.
- **Atuação multiárea:** Artes, Biológicas, Exatas, Humanas, Saúde e Tecnológicas.
- **Coordenadora:** Carmen Verissima Ferreira Halder (2024–2029).
- **Equipe administrativa:** Gislaine Elias Alipio (assistente); Vitoria Esther do
  Rosario Reis (suporte).
- **Endereço:** Av. Erico Veríssimo, 500, Prédio da CDC/GMU, Unicamp (entrada lateral
  direita).
- **Contato:** (19) 3521-4753 · neab@unicamp.br
- Já tem **identidade visual aprovada** e atividades acontecendo (ex.: exposição
  "Bailes Negros", seminários COCEN).

### Objetivos oficiais (norma de criação — Deliberação CONSU-A-007/2024)
1. **Pesquisa** — população afro-brasileira, relações étnico-raciais, ações
   afirmativas e políticas públicas.
2. **Extensão** — projetos cujo cerne é a população afro-brasileira.
3. **Educação** — formar professores da educação básica pra institucionalizar o
   ensino da cultura afro-brasileira (Lei 10.639). *[Está no mandato, mas escola
   NÃO é prioridade do site v1 — input do NEAB.]*
4. **Ações afirmativas** — manutenção e aprimoramento das da Unicamp.
5. **Parcerias** — convênios com setor público, privado e sociedade civil pra
   captar recursos.
6. **Divulgação** — "promover ampla comunicação das atividades do NEAB dentro e fora
   da instituição." → **Este objetivo oficial JUSTIFICA o site.** É o mandato.

### Identidade visual — status
- Identidade aprovada existe, mas **não temos os arquivos**. Estratégia acordada:
  **estudar e propor**, partindo de duas fontes públicas:
  - Logo achável via Google.
  - Instagram **[@neab_unicamp](https://www.instagram.com/neab_unicamp/)** (274
    seguidores, 29 posts) — fonte da estética/tom.
- ⚠️ O Instagram fica atrás de muro de login/JS — **não consegui ler por ferramenta.**
  Preciso que o user compartilhe prints (foto de perfil/logo + alguns posts) pra
  extrair paleta, tipografia e tom. Pendência pra Fase 2.

### Diagnóstico central
O NEAB **NÃO tem site próprio** — só a página dentro do COCEN. É o principal núcleo
sem presença web autônoma. **Isto é greenfield:** a gente constrói do zero, sem dívida
técnica, e o objetivo é dar ao NEAB a mesma autonomia de presença que os núcleos
estabelecidos têm. A página do COCEN não mostra: linhas de pesquisa, projetos,
publicações, agenda estruturada, repositório.

## 3. Referências — como é um site de núcleo maduro

### PAGU (Núcleo de Estudos de Gênero, 1993) — pagu.unicamp.br
Arquitetura de informação:
1. **Institucional** — visão geral, coordenação (atual/anterior), conselho, admin, FAQ, formulários
2. **Pesquisadoras** — permanentes, colaboradoras (internas/externas), sêniors, pós-doc
3. **Pesquisas** — linhas de pesquisa, projetos, iniciação científica
4. **Cadernos Pagu** — revista semestral (política editorial, normas, fluxo)
5. **Biblioteca Beth Lobo** — acervo, banco de teses, novas aquisições
- Extras: Livros Pagu (coleções), Atividades (eventos, Cine Pagu, notícias, "na mídia")
- Recursos: busca, agenda c/ Google Calendar, redes sociais, **acessibilidade (fonte/contraste)**

### NEPO (Núcleo de Estudos de População, 1982) — nepo.unicamp.br
1. **Home** — destaques
2. **NEPO** — sobre, legislação, coordenação, pesquisadores, equipe, biblioteca, TIC, na mídia, vagas
3. **Áreas de pesquisa** — 8 linhas temáticas
4. **Publicações** — textos, livros/revistas, bancos de dados, atlas, anais, relatórios, coleção educativa
5. **Eventos** — atuais e passados, galerias foto/vídeo, emissão de certificado
6. **Pós-graduação** · **Contato**
- Extras: campanhas, dados históricos, footer com acessibilidade + redes

### Referências AFRO-específicas (mais relevantes que PAGU/NEPO p/ repertório)
Fonte: lista do CEA-USP (cea.fflch.usp.br/instituicoes). Núcleos afro pelo Brasil:
ABEÁfrica, CEA/UFMG, NEAF/UFF, CEAO/UFBA, NEAB/UFSCAR, NEAB/UFABC, NEAB/UDESC,
NEAB/UFES, NEAB/UFPR, NIEAAB/UFSC, NEAAB/UNILAB.

**NEAB/UFSCar** (neab.ufscar.br) — referência mais próxima e bem estruturada:
- O Núcleo (quem somos, equipe, áreas de atuação, documentos, história)
- Atividades (grupos de pesquisa, projetos, cursos, parcerias)
- Acervo (biblioteca, coleções, vídeos, Rede NEAB)
- Notícias · Contato
- Conteúdo recente: ativismo antirracista, evento sobre Frantz Fanon, cultura.

**NEAB/UFES** (neab.ufes.br):
- O Núcleo · Pesquisa/Extensão · Anais · Memórias · Fale conosco
- Defende "direito à liberdade de culto, à memória e ao patrimônio cultural
  afro-brasileiro". Coordena seminários nacionais de educação étnico-racial.

### 💡 Insight de design (oportunidade)
A maioria dos núcleos afro federais **herda o template institucional genérico**
(azul + branco padrão universidade) e NÃO tem identidade visual afrocentrada própria.
→ Isso é uma **oportunidade de diferenciação**: o NEAB/Unicamp pode ter uma identidade
genuína, ancorada no repertório estético afro-brasileiro, mantendo a credibilidade
institucional. Não precisa parecer "mais um site .br de universidade". Equilíbrio:
personalidade afrocentrada + códigos de confiança acadêmica.

### Padrão comum a destilar pro NEAB
- **Institucional / Sobre** (missão, histórico, legislação de criação, coordenação)
- **Pessoas** (pesquisadores + equipe, com Lattes/ORCID/Scholar)
- **Pesquisa** (linhas + projetos)
- **Publicações** (o que o núcleo produz)
- **Eventos / Atividades** (agenda + memória, com galerias e certificados)
- **Contato**
- **Acessibilidade** como requisito de base (contexto universitário público)

## 4. Implicações pro projeto (a confirmar com o NEAB)
- Como núcleo novo, talvez não haja volume ainda pra todas as seções (ex.: revista
  própria). Melhor um site que **começa enxuto e cresce** — arquitetura que comporta
  Publicações/Linhas de pesquisa mesmo que comecem pequenas.
- Identidade visual já existe → **partir dela**, não inventar.
- Padrão Unicamp/COCEN dá baliza de credibilidade, mas o NEAB pode (e deve) ter
  personalidade própria — núcleo de estudos afro-brasileiros tem repertório estético
  e político próprio.
- Acessibilidade e provavelmente **bilíngue/conteúdo público** a considerar.

## 5. Decisões definidas (input do NEAB)

- **Objetivo nº1: dar existência / visibilidade.** O site é o "cartão de existência"
  do núcleo novo: mostrar que o NEAB existe, o que é e o que faz. Presença
  institucional vem antes de tudo. → Implica clareza e acolhimento, não um portal
  acadêmico denso. A home tem que responder em segundos "o que é isto?".
- **Público (3 frentes, não-especialistas inclusos):**
  1. Comunidade acadêmica (estudantes/pesquisadores, Unicamp e fora)
  2. Comunidade externa / movimento negro / coletivos
  3. Instituições / parceiros / financiadores
  → NÃO inclui escolas como prioridade → menos material didático (Lei 10.639),
  mais institucional + vitrine de pesquisa + credibilidade pra parceria.
  → Público misto exige linguagem que funciona pra quem é da área E pra quem não é.
- **Manutenção: equipe do NEAB sozinha (não-técnica).** → **REQUISITO FORTE: CMS/painel
  admin amigável.** Não pode ser site que só dev atualiza. Isso é o maior direcionador
  técnico do projeto.

### Implicações de arquitetura/tecnologia
- Site precisa de **camada de administração** pra: notícias/eventos, pessoas,
  publicações, linhas de pesquisa. Conteúdo editável sem código.
- Opções de stack a avaliar na Fase 2/3 considerando que mantenedor é não-técnico:
  CMS hospedado, headless CMS + front, git-based CMS (ex. Decap), ou padrão
  HTML + Firebase (já usado pelo user em outro projeto). **Decisão depende da infra
  que a Unicamp/COCEN oferece** (ver lacunas abaixo).

## 6. Lacunas ainda abertas (antes de desenhar)
- [ ] **Infra/hospedagem:** o que a Unicamp/COCEN dá? (domínio neab.unicamp.br?
      consegue rodar Node/PHP/banco, ou é só estático? isso decide o tipo de CMS)
- [ ] **Identidade visual aprovada:** logo, cores, tipografia — precisamos dos arquivos
- [ ] **Conteúdo real existente:** linhas de pesquisa, projetos, pesquisadores,
      eventos já realizados — pra mapear o que entra no v1
- [ ] Dor específica que motivou o site (o que falta hoje na página da COCEN)
