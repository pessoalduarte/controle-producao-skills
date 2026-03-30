# Mapa de Skills por Situacao

> Consulte este mapa ANTES de cada acao para identificar skills relevantes.
> Se uma situacao se encaixar, INVOQUE a skill correspondente.

---

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

### dev-browser vs playwright:
| Ferramenta | Como funciona | Usar quando |
|------------|--------------|-------------|
| **dev-browser** | Analisa o CODIGO/DOM real via JavaScript sandboxed | Analise de codigo, debug HTML/CSS/JS, extracao de dados, testes funcionais, automacao de formularios |
| **playwright** | Captura SCREENSHOTS e usa IA para analisar a imagem | Verificacao visual (layout, design, responsividade), testes de regressao visual |

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
| Encerrar expediente | production-tracker - "encerrar expediente" |
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
