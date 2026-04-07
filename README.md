# Intranet Classe II — 3° Batalhão de Suprimento

Sistema de intranet para gerenciamento operacional da Seção Classe II do 3° Batalhão de Suprimento do Exército Brasileiro.

---

## Sobre o Projeto

A **Classe II** é responsável por prover as Organizações Militares (OMs) integrantes da 3ª Região Militar com suprimentos Classe II — uniformes, tecidos, aviamentos, bandeiras, flâmulas, insígnias e demais materiais correlatos.

Esta intranet centraliza os processos operacionais da seção em uma interface web moderna, profissional e responsiva, facilitando o dia-a-dia do efetivo.

---

## Funcionalidades

### Painel de Controle (Dashboard)
- Cards de métricas: itens em estoque, ordens pendentes, efetivo presente, entregas no mês
- Ações rápidas para navegação entre módulos

### Gerenciamento de Efetivo
- Escala de serviço com integração Google Sheets
- Consulta de dados cadastrais do efetivo
- Controle de férias *(em breve)*

### Seção de Recebimento
- Registro de recebimento de materiais com nota fiscal
- Acompanhamento de materiais em verificação quantitativa
- Consulta de estoque atual *(em breve)*

### Seção de Expedição
- Registro de novas expedições *(em breve)*
- Rastreamento de expedições em andamento *(em breve)*
- Histórico de expedições *(em breve)*

### Formulários de Controle
- Formulário de materiais em contagem
- Formulário de recebimento de materiais
- Guia de remessa para expedição *(em breve)*

### Relatórios e Registros
- Relatório mensal consolidado *(em breve)*
- Livro de registro cronológico *(em breve)*
- Geração de relatórios para impressão *(em breve)*

---

## Estrutura do Projeto

```
3bsup-classe2/
├── index.html                    # Página principal
├── .gitignore
├── README.md
└── src/
    ├── assets/
    │   └── img/
    │       └── logo-cl2.png      # Brasão da Classe II
    └── css/
        ├── main.css              # Arquivo de importação central
        ├── responsive.css        # Media queries
        ├── base/
        │   ├── reset.css         # Normalização CSS
        │   ├── variables.css     # Design tokens (cores EB, sombras, etc.)
        │   └── typography.css    # Tipografia global
        ├── components/
        │   ├── buttons.css       # Botões e badges
        │   └── cards.css         # Cards de estatísticas e gerenciamento
        ├── layout/
        │   ├── header.css        # Cabeçalho, navegação e menu mobile
        │   ├── footer.css        # Rodapé institucional
        │   └── sections.css      # Containers e layout de seções
        └── pages/
            ├── dashboard.css     # Grid do painel de controle
            └── management.css    # Grid de gerenciamento
```

---

## Paleta de Cores

| Cor | Hex | Uso |
|-----|-----|-----|
| Verde Oliva | `#3d5a1e` | Cor primária — identidade do Exército Brasileiro |
| Verde Escuro | `#2a3f15` | Hover e elementos de destaque |
| Verde Muito Escuro | `#1d2b10` | Header e footer |
| Dourado | `#c5a028` | Acentos e ícones — referência ao brasão |
| Bege | `#f0efe8` | Fundo principal |
| Bege Escuro | `#e8e6da` | Fundo alternado entre seções |

---

## Tecnologias

- **HTML5** — Estrutura semântica
- **CSS3** — Estilização modular com CSS Custom Properties (variáveis)
- **Font Awesome 6** — Ícones vetoriais
- **Google Sheets** — Integração para planilhas de efetivo

---

## Como Usar

1. Clone o repositório:
   ```bash
   git clone https://github.com/Giovanne-Portella/3bsup-classe2.git
   ```

2. Abra o arquivo `index.html` no navegador ou utilize um servidor local:
   ```bash
   # Com Python
   python -m http.server 8080

   # Com Node.js (npx)
   npx serve .
   ```

3. Acesse `http://localhost:8080`

---

## Branches

| Branch | Descrição |
|--------|-----------|
| `main` | Produção — código estável e validado |
| `hml` | Homologação — testes e validação antes de ir para produção |
| `dev` | Desenvolvimento — novas funcionalidades em andamento |

### Fluxo de trabalho

```
dev → hml → main
```

1. Desenvolva novas features na branch `dev`
2. Teste e valide em `hml`
3. Merge para `main` quando aprovado

---

## Contribuição

1. Crie uma branch a partir de `dev`:
   ```bash
   git checkout dev
   git checkout -b feature/nome-da-feature
   ```

2. Faça suas alterações e commit:
   ```bash
   git add .
   git commit -m "feat: descrição da alteração"
   ```

3. Envie e abra um Pull Request para `dev`:
   ```bash
   git push origin feature/nome-da-feature
   ```

### Padrão de Commits

| Prefixo | Uso |
|---------|-----|
| `feat:` | Nova funcionalidade |
| `fix:` | Correção de bug |
| `refactor:` | Refatoração de código |
| `style:` | Alterações visuais/CSS |
| `docs:` | Documentação |
| `chore:` | Tarefas de manutenção |

---

## Autor

**Cabo Portella** — Seção Classe II / 3° Batalhão de Suprimento

---

## Licença

Projeto de uso interno — Exército Brasileiro.
