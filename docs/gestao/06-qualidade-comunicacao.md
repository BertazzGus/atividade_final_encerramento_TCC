# 06 — Plano de Qualidade e Plano de Comunicação

> **Aviso:** dados simulados para fins didáticos.

## Plano de qualidade

| Critério | Como será verificado | Quando | Resultado simulado |
|---|---|---|---|
| Requisitos funcionais | Checklist e testes manuais de autenticação, clientes, veículos, estoque, orçamento, ordem de serviço, faturamento e relatórios | Cada incremento e entrega | Atendido, exceto KPIs (removido) |
| Isolamento entre tenants | Testes tentando acessar dados de outro tenant; revisão de filtros e permissões | Alterações de segurança ou persistência | Zero acessos cruzados nos testes |
| Defeitos e código | Testes automatizados, revisão de código, lint do frontend e build do backend | Cada merge ou versão candidata | 2 defeitos críticos corrigidos antes da homologação |
| Artigo SBC | Conferência de seções, citações, referências, tabelas, paginação e revisão textual | Cada revisão e submissão | Aprovado após 2 revisões |
| Reprodutibilidade | Instruções atualizadas, variáveis documentadas e execução em ambiente limpo | Demonstração final | Executado em ambiente limpo na homologação |

## Plano de comunicação

| Parte interessada | Informação | Frequência | Canal |
|---|---|---|---|
| Orientador | Progresso, riscos, decisões, impedimentos e versões para revisão | Semanal | Reunião e resumo escrito |
| Banca | Problema, objetivos, método, resultados, limitações e demonstração | Marcos | Artigo, slides e apresentação |
| Coordenação | Prazos, documentos exigidos e situação das etapas | Calendário | Sistema acadêmico |
| Usuários (oficina piloto) | Fluxos, necessidades, limitações e validação das telas | Validações | Entrevista ou demonstração registrada |
| Desenvolvedor | Tarefas, decisões, riscos, defeitos e próximos passos | Diário | Backlog e diário do projeto |

**Controle contra ruídos:** decisões e mudanças são registradas por escrito. Cada reunião com o orientador termina com tarefas, responsáveis e prazo.
