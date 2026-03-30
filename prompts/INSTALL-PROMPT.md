# Prompt de Instalacao — Production Tracker v2

> Use este prompt ao iniciar um novo projeto para configurar o production-tracker
> de forma completa e profissional.

---

## Prompt para colar no inicio de cada novo projeto:

```
Se a skill production-tracker NAO estiver instalada, instale:
npx skills add https://github.com/pessoalduarte/controle-producao-skills --agent claude-code --skill '*' -y

Ative a skill production-tracker para este projeto. Configure o controle de producao profissional com as seguintes regras:

1. SEMPRE registre todas as atividades com timestamp (America/Sao_Paulo)
2. Cada tarefa DEVE ter hora de inicio, hora de fim e duracao calculada
3. Ao final do expediente, gere relatorio completo com:
   - Dados do contratante e contratado
   - Composicao detalhada de horas por atividade
   - Metricas de producao (commits, arquivos, linhas)
   - Justificativa tecnica de honorarios
   - PDF formatado profissionalmente

Se nao existir o arquivo .claude/production/project-config.json, pergunte:
- Nome da empresa contratada
- Nome do programador responsavel
- Nome do cliente (pessoa)
- Nome da empresa do cliente
- Nome/descricao do projeto
- Modelo de cobranca (por hora, por projeto, mensal)

O relatorio serve como comprovante profissional de trabalho para justificativa de honorarios. Deve ser claro, detalhado e tecnico o suficiente para que o contratante entenda o valor do trabalho realizado.

Inicie o rastreamento AGORA — registre esta sessao como primeiro registro do dia.
```

---

## Dica: Para projetos recorrentes

Se voce ja tem o `project-config.json` de um projeto anterior e quer reutilizar
o formato, basta copiar e ajustar os dados do novo cliente.
