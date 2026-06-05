# Site do NEAB Unicamp — mockup

Protótipo da home do **Núcleo de Estudos Afro-Brasileiros (NEAB)** da Unicamp.
Página estática (HTML/CSS/JS vanilla, sem build), feita para crítica e validação da
direção antes de construir o site final.

## Estrutura
- `index.html` — a home
- `neab.png`, `unicamp-logo.png` — logos
- `img/` — fotos de exemplo (Wikimedia Commons, livres) usadas como **placeholder**
- `CONHECIMENTO.md` — pesquisa sobre COCEN/NEAB e referências
- `ARQUITETURA.md` — arquitetura de informação (mapa do site, modelo de conteúdo)
- `IDENTIDADE-VISUAL.md` — identidade extraída do Instagram do NEAB
- `DIRECAO-VISUAL.md` — sistema de design e histórico de iterações

## Rodar localmente
Abra `index.html` no navegador, ou sirva a pasta:

```
python3 -m http.server 8000
```

e acesse http://localhost:8000

## Avisos (importante para a crítica)
- As fotos em `img/` são **exemplos livres do Wikimedia Commons**, só para demonstrar o
  layout. Devem ser substituídas pelas **fotos reais do NEAB**.
- As fontes vêm do Google Fonts (precisa de internet para renderizar).
- Conteúdo (notícias, eventos, equipe) é de demonstração.
