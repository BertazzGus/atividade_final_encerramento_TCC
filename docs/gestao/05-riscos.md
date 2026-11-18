# 05 — Registro de Riscos

> **Aviso:** dados simulados para fins didáticos. Status "materializado" é simulado.

| # | Risco | Categoria | Prob. | Impacto | Resposta planejada | Situação final (simulada) |
|---|---|---|---|---|---|---|
| R1 | API de CEP indisponível ou alterada | Externo | Média | Médio | Mitigar com preenchimento manual e tratamento de erro | **Materializado** em testes; resposta de mitigação aplicada (ver `08-log-mudancas.md`) |
| R2 | Falha no isolamento multi-tenant | Interno | Baixa | Alto | Evitar com revisão de filtros, testes de autorização e validação de acesso cruzado | Não materializado |
| R3 | Sobrecarga com trabalho e disciplinas | Interno | Alta | Alto | Mitigar com cronograma semanal, escopo mínimo e reserva para correções | **Parcialmente materializado**: atraso de 1 semana na homologação |
| R4 | Indisponibilidade do orientador | Externo | Média | Médio | Mitigar enviando pautas e versões com antecedência e registrando decisões | Não materializado |
| R5 | Retrabalho após qualificação ou banca | Externo | Média | Alto | Mitigar com backlog priorizado, documentação atualizada e reserva no cronograma | Não materializado |
| R6 | Defeito crítico próximo da apresentação | Interno | Média | Alto | Mitigar com testes automatizados, validação manual e build em ambiente limpo | Não materializado |
| R7 | Compatibilidade do ambiente de homologação com a oficina piloto | Interno | — | Médio | Não estava previsto | **Identificado durante a execução** (risco não registrado na linha de base) |

## Riscos prioritários
Sobrecarga de tempo (R3), retrabalho solicitado pela avaliação (R5) e falha de isolamento multi-tenant (R2). O R2 tem probabilidade menor, mas impacto alto: uma falha comprometeria a segurança e a principal característica arquitetural do produto.

## Observação sobre R7
O risco R7 não constava no registro original. Foi identificado durante a execução e tratado como lição aprendida (ver `11-licoes-aprendidas.md`).
