# controle-producao-skills

Skills para Claude Code: controle de producao profissional, mapeamento de skills por situacao e setup automatizado de novos projetos.

## O que e isso?

Um conjunto de ferramentas para desenvolvedores que usam Claude Code e precisam de:

- **Controle de producao** com timestamps, composicao de horas e relatorios PDF
- **Mapeamento de skills** por situacao (qual skill usar em cada cenario)
- **Setup automatizado** de novos projetos com verificacao de skills obrigatorias
- **Justificativa profissional** de honorarios para contratantes

## Instalacao

```bash
npx skills add https://github.com/pessoalduarte/controle-producao-skills --agent claude-code --skill '*' -y
```

## Como usar

### 1. Setup completo de novo projeto

Cole o conteudo de [`prompts/SETUP-NOVO-PROJETO.md`](prompts/SETUP-NOVO-PROJETO.md) na primeira mensagem ao iniciar um novo projeto no Claude Code. Ele faz:

1. Verifica e instala skills obrigatorias
2. Configura o production-tracker com dados do contrato
3. Cria o mapa de skills por situacao (`.claude/SKILLS-MAP.md`)
4. Inicia o rastreamento de producao

### 2. Apenas ativar o production-tracker

Cole o conteudo de [`prompts/INSTALL-PROMPT.md`](prompts/INSTALL-PROMPT.md) para configurar apenas o controle de producao.

## Estrutura

```
controle-producao-skills/
├── skills/
│   └── production-tracker/
│       └── SKILL.md                 <- Skill principal
├── prompts/
│   ├── SETUP-NOVO-PROJETO.md        <- Prompt completo de setup
│   └── INSTALL-PROMPT.md            <- Prompt simples do tracker
├── templates/
│   ├── project-config.json          <- Template de configuracao do contrato
│   ├── pdf-config.json              <- Template de estilo do PDF
│   └── SKILLS-MAP.md                <- Mapa completo de skills por situacao
├── LICENSE
└── README.md
```

## Funcionalidades

### Production Tracker v2

- Registro automatico com timestamps (America/Sao_Paulo)
- Dados profissionais: contratada, contratante, projeto
- Cada atividade com hora de inicio, fim e duracao
- Composicao detalhada de horas por atividade
- Justificativa tecnica de honorarios
- Geracao de PDF formatado (A4, header/footer, tabelas estilizadas)
- Suporte a virada de meia-noite (expediente continuo)
- Relatorios semanais e mensais sob demanda
- Integracao com napkin, GSD, commit-commands e outras skills

### Comandos

| Comando | Acao |
|---------|------|
| "relatorio de producao" | Finalizar e gerar PDF |
| "resumo do dia" | Timeline resumida |
| "encerrar expediente" | Metricas + PDF + pendencias |
| "producao da semana" | Compilar ultimos 7 dias |
| "composicao de horas" | Tabela detalhada |

### Skills Map

Mapeamento de 150+ skills em 17 categorias incluindo: Planejamento, Desenvolvimento, UI/UX, GSD, Pesquisa, DevOps, Testes/QA, Marketing, CRO, Dados, Media, Producao, Seguranca, Equipe/Agentes e Utilitarios.

Destaque: distincao clara entre **dev-browser** (analisa CODIGO/DOM) e **playwright** (analisa VISUAL/screenshots).

### Skills obrigatorias verificadas no setup

| Skill | Repo |
|-------|------|
| ralph | snarktank/ralph |
| superpowers | obra/superpowers |
| everything-claude-code | affaan-m/everything-claude-code |
| ui-ux-pro-max | nextlevelbuilder/ui-ux-pro-max-skill |
| obsidian-skills | kepano/obsidian-skills |
| get-shit-done | gsd-build/get-shit-done |
| interface-design | Dammyjay93/interface-design |
| napkin | blader/napkin |
| marketingskills | coreyhaines31/marketingskills |
| aiox-core | Synkraai/aiox-core |
| claude-mem | thedotmack/claude-mem |
| skills-best-practices | mgechev/skills-best-practices |
| dev-browser | SawyerHood/dev-browser |

## Contribuindo

Melhorias sao bem-vindas! Este repositorio evolui a cada projeto.

## Licenca

MIT
