# Estrutura de Pastas do Projeto Blog

## Estrutura Final (Jekyll + GitHub Pages)

```
blog-project/
│
├── _posts/                    # Todos os artigos
│   ├── finance/              # Artigos de finanças
│   │   ├── 2026/
│   │   │   ├── 01/
│   │   │   │   ├── 2026-01-27-passive-income-for-developers.md
│   │   │   │   └── 2026-01-28-investing-basics.md
│   │   │   └── 02/
│   │   │       └── ...
│   │   └── 2027/
│   │       └── ...
│   │
│   ├── dev/                  # Artigos de desenvolvimento
│   │   ├── 2026/
│   │   │   ├── 01/
│   │   │   │   ├── 2026-01-27-rest-api-best-practices.md
│   │   │   │   └── 2026-01-28-python-optimization.md
│   │   │   └── 02/
│   │   │       └── ...
│   │   └── 2027/
│   │       └── ...
│   │
│   ├── study/                # Artigos de estudos
│   │   ├── 2026/
│   │   │   ├── 01/
│   │   │   │   ├── 2026-01-27-efficient-study-methods.md
│   │   │   │   └── 2026-01-28-exam-preparation.md
│   │   │   └── 02/
│   │   │       └── ...
│   │   └── 2027/
│   │       └── ...
│   │
│   └── profit/               # Artigos de rentabilidade
│       ├── 2026/
│       │   ├── 01/
│       │   │   ├── 2026-01-27-seo-basics.md
│       │   │   └── 2026-01-28-freelancing-tips.md
│       │   └── 02/
│       │       └── ...
│       └── 2027/
│           └── ...
│
├── _layouts/                 # Layouts customizados (opcional)
│   ├── default.html
│   ├── post.html
│   └── page.html
│
├── _includes/                # Includes customizados (opcional)
│   ├── header.html
│   ├── footer.html
│   └── nav.html
│
├── _sass/                    # Estilos customizados (opcional)
│   ├── _base.scss
│   └── _custom.scss
│
├── css/                      # Arquivos CSS
│   └── style.scss
│
├── js/                       # Arquivos JavaScript (opcional)
│   └── main.js
│
├── images/                   # Imagens do blog
│   ├── finance/
│   ├── dev/
│   ├── study/
│   └── profit/
│
├── _config.yml               # Configuração do Jekyll
├── index.html                # Pagina inicial
├── about.html                # Pagina sobre
├── contact.html              # Pagina de contato
├── finance.html              # Pagina index de finanças
├── dev.html                  # Pagina index de dev
├── study.html                # Pagina index de estudo
├── profit.html               # Pagina index de profit
├── CNAME                     # Dominio personalizado (depois de comprar)
└── README.md                 # Documentação do projeto
```

## Estrutura Inicial (para comecar)

Para comecar, vamos criar uma estrutura minima:

```
blog-project/
│
├── _posts/
│   ├── finance/
│   ├── dev/
│   ├── study/
│   └── profit/
│
├── images/
│
├── _config.yml
├── index.html
└── README.md
```

## Por que esta estrutura?

### _posts/ organizado por nicho
- Facilita navegacao
- Facilita geracao automatica de paginas de indice por nicho
- Facilita analise de metricas por nicho

### Date-nome-arquivo.md
- Jekyll exige este formato para posts
- Organizacao cronologica automatica
- URL limpa (ex: /finance/2026/01/27/passive-income-for-developers)

### Separação por nicho
- Permite focar em um nicho por vez
- Facilita expansao futura
- Permite remover/renomear nichos sem afetar outros

### Imagens separadas
- Facilita otimizacao (WebP, lazy loading)
- Facilita backup
- Facilita mover para CDN depois

## Proxima Escada

Apos criar esta estrutura, vamos:
1. Criar o arquivo _config.yml
2. Criar o primeiro artigo modelo
3. Configurar GitHub Pages
