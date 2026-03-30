# Setup Completo para Novos Projetos — Production Tracker v2

> Cole o prompt da ETAPA UNICA ao iniciar qualquer novo projeto.
> Ele verifica skills, instala faltantes, configura production-tracker
> e cria o mapa de skills por situacao — tudo auto-contido.
>
> Nenhuma referencia a outros projetos ou clientes. Generico e reutilizavel.

---

## PROMPT DE SETUP (copiar tudo entre os delimitadores ```):

```
# SETUP INICIAL DE PROJETO

Execute as 4 etapas abaixo na ordem, sem pular nenhuma.

## ETAPA 1 — VERIFICACAO DE SKILLS OBRIGATORIAS

Verifique se TODAS as skills abaixo estao instaladas. Para cada uma, procure
pelo nome na lista de skills disponiveis. Se NAO encontrar, instale.

REGRA DE INSTALACAO:
- Usar SEMPRE: npx skills add <repo> --agent claude-code --skill '*' -y
- NUNCA usar: --all (cria pastas desnecessarias na raiz)
- Para repos com subdiretorios: adicionar --full-depth
- Apos instalar: verificar se pastas indevidas foram criadas na raiz e remove-las
- Apenas .claude/skills/ e necessario para Claude Code

### Skills Obrigatorias (verificar/instalar):

| Skill esperada | Repo (instalar se faltar) |
|---|---|
| ralph | https://github.com/snarktank/ralph |
| brainstorming, systematic-debugging | https://github.com/obra/superpowers |
| configure-ecc | https://github.com/affaan-m/everything-claude-code |
| ui-ux-pro-max | https://github.com/nextlevelbuilder/ui-ux-pro-max-skill |
| obsidian-bases, obsidian-cli | https://github.com/kepano/obsidian-skills |
| gsd:progress, gsd:plan-phase | https://github.com/gsd-build/get-shit-done |
| interface-design | https://github.com/Dammyjay93/interface-design |
| napkin | https://github.com/blader/napkin |
| marketing-ideas, marketing-psychology | https://github.com/coreyhaines31/marketingskills |
| aiox-architect, aiox-pm, aiox-dev | https://github.com/Synkraai/aiox-core |
| mem-search, timeline-report | https://github.com/thedotmack/claude-mem |
| skill-creator | https://github.com/mgechev/skills-best-practices |
| dev-browser | https://github.com/SawyerHood/dev-browser |
| production-tracker | Ja deve existir em ~/.claude/skills/ |

### Plugins Obrigatorios (verificar nos plugins instalados):
- playwright (automacao visual de browser)
- superpowers (brainstorming, debugging, worktrees, etc)
- supabase (banco de dados)
- context7 (documentacao atualizada de bibliotecas)
- figma (design system)
- commit-commands (git workflow)
- code-review (revisao de codigo)
- pr-review-toolkit (revisao de PR completa)
- feature-dev (desenvolvimento guiado de features)

Apresente relatorio:
- ✅ [nome] — instalada
- ❌ [nome] — FALTANDO → instalando...

---

## ETAPA 2 — CONFIGURACAO DO PRODUCTION TRACKER

Ative a skill production-tracker para este projeto.

Se nao existir .claude/production/project-config.json, pergunte:
1. Qual o nome da sua empresa? (contratada)
2. Qual o seu nome completo? (programador responsavel)
3. Qual o nome do cliente? (pessoa fisica)
4. Qual o nome da empresa do cliente? (contratante)
5. Qual o nome/descricao do projeto?
6. Qual o modelo de cobranca? (por hora / por projeto / mensal)
7. Alguma observacao importante? (opcional)

Salve as respostas em .claude/production/project-config.json
Crie tambem .claude/production/pdf-config.json com a configuracao visual do PDF.
Registre esta sessao como primeiro registro do dia com timestamp (America/Sao_Paulo).

---

## ETAPA 3 — CRIAR MAPA DE SKILLS POR SITUACAO

Crie o arquivo `.claude/SKILLS-MAP.md` com o conteudo abaixo.
Este mapa e o guia para saber AUTOMATICAMENTE qual skill usar em cada situacao.
Consulte-o ANTES de cada acao. Se uma situacao se encaixar, INVOQUE a skill.

### Conteudo do SKILLS-MAP.md:

# Mapa de Skills por Situacao

> Consulte ANTES de cada acao. Se encaixar, INVOQUE a skill correspondente.

## Planejamento e PRD
| Situacao | Skill |
|----------|-------|
| Criar PRD completo | prd, aiox-pm |
| Planejar feature complexa | blueprint, make-plan |
| Pesquisa de mercado/competidores | market-research, aiox-analyst |
| Definir arquitetura de sistema | architect-first, aiox-architect |
| Decisao tecnica importante | architecture-decision-records |
| Brainstorm de ideias | superpowers:brainstorming |
| Plano multi-sessao/multi-etapa | blueprint |
| Otimizar prompts para agentes | prompt-optimizer |

## Desenvolvimento
| Situacao | Skill |
|----------|-------|
| Implementar feature guiada | feature-dev:feature-dev |
| Escrever testes primeiro (TDD) | tdd-workflow |
| Debug de bug | superpowers:systematic-debugging, gsd:debug |
| Code review de PR | code-review:code-review, pr-review-toolkit:review-pr |
| Padroes de codigo universais | coding-standards |
| API REST design | api-design |
| Backend patterns | backend-patterns |
| Frontend patterns (React/Next) | frontend-patterns |
| Database design (Postgres) | postgres-patterns, aiox-data-engineer |
| Migracoes de banco | database-migrations |
| Integrar Claude API / Anthropic SDK | claude-api |
| Criar MCP server customizado | mcp-server-patterns, mcp-builder |
| Executar plano com subagentes | do |
| Qualidade de codigo automatica | plankton-code-quality |

## UI/UX e Design
| Situacao | Skill |
|----------|-------|
| Dashboard/painel admin | interface-design |
| UI/UX completo (50+ estilos) | ui-ux-pro-max |
| Landing page / frontend premium | frontend-design:frontend-design |
| Design system Figma | figma:figma-generate-library |
| Implementar design do Figma | figma:figma-implement-design |
| UX research e design workflow | aiox-ux-design-expert |
| Revisao de UI (acessibilidade) | web-design-guidelines |
| Otimizar formularios (CRO) | form-cro |
| Auditoria de click-path/estado | click-path-audit |
| Gerar slides/apresentacoes HTML | frontend-slides |

## Gestao de Projeto (GSD)
| Situacao | Skill |
|----------|-------|
| Iniciar novo projeto | gsd:new-project |
| Ver progresso atual | gsd:progress |
| Planejar fase | gsd:plan-phase |
| Executar fase | gsd:execute-phase |
| Pausar trabalho (context handoff) | gsd:pause-work |
| Retomar trabalho | gsd:resume-work |
| Debug sistematico | gsd:debug |
| Adicionar fase ao roadmap | gsd:add-phase |
| Modo autonomo (todas as fases) | gsd:autonomous |
| Verificar trabalho entregue | gsd:verify-work |
| Estatisticas do projeto | gsd:stats |
| Checklist generico | checklist-runner |

## Documentacao e Pesquisa
| Situacao | Skill |
|----------|-------|
| Pesquisa tecnica profunda | tech-search, deep-research |
| Busca neural (Exa) | exa-search |
| Docs atualizadas de bibliotecas | documentation-lookup (Context7) |
| Extrair conteudo limpo de pagina | defuddle |
| Escrever artigo/guia/tutorial | article-writing |
| Explorar codebase desconhecido | smart-explore, codebase-onboarding |
| Memoria persistente entre sessoes | napkin, mem-search |
| Criar diagrama/mapa visual | json-canvas |
| Gerar relatorio de timeline | timeline-report |

## DevOps e Deploy
| Situacao | Skill |
|----------|-------|
| Docker/Docker Compose | docker-patterns |
| CI/CD pipelines | deployment-patterns |
| Git commit | commit-commands:commit |
| Commit + push + PR | commit-commands:commit-push-pr |
| Limpar branches deletados | commit-commands:clean_gone |
| Runtime Bun (alternativa a Node) | bun-runtime |

## Testes, QA e Automacao de Browser

### dev-browser vs playwright — REGRA CLARA:

| Ferramenta | Como funciona | Usar quando |
|------------|--------------|-------------|
| **dev-browser** | Analisa o CODIGO/DOM real via JavaScript sandboxed | Analise de codigo, debug HTML/CSS/JS, extracao de dados, testes funcionais, automacao de formularios, inspecao de elementos |
| **playwright** | Captura SCREENSHOTS e usa IA para analisar a imagem | Verificacao visual (layout, design, responsividade), testes de regressao visual, comparacao de screenshots |

**Regra:** dev-browser = entender o CODIGO. playwright = ver o VISUAL.

| Situacao | Skill |
|----------|-------|
| Analise de codigo de pagina | dev-browser |
| Testes end-to-end (E2E) | e2e-testing + dev-browser |
| Debug de HTML/CSS/JS | dev-browser |
| Extracao de dados de paginas | dev-browser |
| Automacao de formularios | dev-browser |
| Verificacao visual (layout) | playwright (screenshot + IA) |
| Testes de regressao visual | playwright |
| Validacao pos-deploy | playwright (agent-browser-verify) |
| Python tests | python-testing |
| Testes de regressao para IA | ai-regression-testing |
| Framework de avaliacao formal | eval-harness |
| Comparar agentes | agent-eval |
| Verificacao final antes de entregar | superpowers:verification-before-completion |
| Verificacao completa (loop) | verification-loop |

## Marketing e Conteudo
| Situacao | Skill |
|----------|-------|
| Ideias de marketing | marketing-ideas |
| Copywriting (paginas, CTAs) | copywriting |
| Editar/revisar copy existente | copy-editing |
| SEO audit do site | seo-audit |
| SEO para AI (ser citado por LLMs) | ai-seo |
| Email marketing / drip campaigns | email-sequence |
| Redes sociais | social-content |
| Crosspost multi-plataforma | crosspost |
| Psicologia de marketing | marketing-psychology |
| Estrategia de conteudo | content-strategy |
| Criar conteudo multi-plataforma | content-engine |
| Anuncios pagos (Google, Meta) | paid-ads |
| Criativos de anuncio | ad-creative |
| Cold email B2B | cold-email |
| SEO programatico (escala) | programmatic-seo |
| Paginas de comparacao/alternativas | competitor-alternatives |
| Lead magnets | lead-magnets |
| Schema markup (dados estruturados) | schema-markup |
| Arquitetura do site (hierarquia) | site-architecture |
| Estrategia de lancamento | launch-strategy |
| Precificacao e monetizacao | pricing-strategy |
| Contexto de product marketing | product-marketing-context |
| Programa de indicacao/referral | referral-program |
| Free tool strategy | free-tool-strategy |
| Revenue operations | revops |
| Sales enablement (material vendas) | sales-enablement |
| Investidor (pitch deck, one-pager) | investor-materials, investor-outreach |

## CRO (Otimizacao de Conversao)
| Situacao | Skill |
|----------|-------|
| Otimizar pagina de marketing | page-cro |
| Otimizar formularios | form-cro |
| Otimizar signup/registro | signup-flow-cro |
| Otimizar onboarding pos-signup | onboarding-cro |
| Otimizar paywall/upgrade | paywall-upgrade-cro |
| Otimizar popups/modals | popup-cro |
| Reduzir churn/cancelamento | churn-prevention |
| Setup de A/B test | ab-test-setup |
| Analytics e tracking | analytics-tracking |

## Dados e Automacao
| Situacao | Skill |
|----------|-------|
| Scraper de dados automatizado | data-scraper-agent |
| Otimizar custos de LLM | cost-aware-llm-pipeline |
| Regex vs LLM para parsing | regex-vs-llm-structured-text |

## Media e Geracao de Conteudo
| Situacao | Skill |
|----------|-------|
| Gerar imagem/video/audio (fal.ai) | fal-ai-media |
| Editar video com IA | video-editing |
| Video/audio processing | videodb |

## Producao e Relatorios
| Situacao | Skill |
|----------|-------|
| Registro de producao | production-tracker (SEMPRE ATIVA) |
| Relatorio de timeline do projeto | timeline-report |
| Encerrar expediente | production-tracker → "encerrar expediente" |
| Compactacao estrategica de contexto | strategic-compact |

## Seguranca
| Situacao | Skill |
|----------|-------|
| Revisao de seguranca de codigo | security-review |
| Scan de configuracao Claude | security-scan |

## Equipe e Agentes
| Situacao | Skill |
|----------|-------|
| Montar equipe de agentes | team-builder, aiox-squad-creator |
| Orquestrar agentes (master) | aiox-master |
| Product Manager | aiox-pm |
| Product Owner | aiox-po |
| QA/Testes | aiox-qa |
| Scrum Master | aiox-sm |
| DevOps/Repositorio | aiox-devops |
| Full Stack Dev | aiox-dev |
| Loops autonomos de agentes | autonomous-loops, continuous-agent-loop |
| Multi-agentes em paralelo | claude-devfleet, dmux-workflows |
| Engenharia agentica | agentic-engineering |
| Modelo AI-first para equipe | ai-first-engineering |
| Otimizar action space de agentes | agent-harness-construction |
| Melhorar retrieval de contexto | iterative-retrieval |
| Contexto SYNAPSE engine | synapse |

## Skills de Gestao e Utilitarios
| Situacao | Skill |
|----------|-------|
| Criar nova skill | skill-creator |
| Pesquisa antes de codar | search-first |
| Auditar uso de contexto | context-budget |
| Aprendizado continuo | continuous-learning, continuous-learning-v2 |
| Revisar CLAUDE.md | claude-md-management:revise-claude-md |
| Configurar ECC | configure-ecc |
| Extrair regras de skills | rules-distill |

---

## ETAPA 4 — VERIFICACAO FINAL

Apos completar as etapas acima, apresente:

1. Relatorio de skills instaladas vs faltantes
2. Confirmacao do production-tracker configurado com dados do contrato
3. Confirmacao do SKILLS-MAP.md criado em .claude/
4. Primeiro registro de producao do dia com timestamp

Inicie o rastreamento de producao AGORA.
```

---

## Como usar

1. Abra um novo projeto no Claude Code
2. Cole o prompt acima inteiro na primeira mensagem
3. O agente verifica, instala e configura tudo automaticamente
4. A partir dai, as skills sao usadas automaticamente conforme o SKILLS-MAP.md
5. Ao final do expediente, diga "encerrar expediente" para gerar o relatorio PDF
