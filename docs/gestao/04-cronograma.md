# 04 — Cronograma e Diagrama de Rede

> **Aviso:** dados simulados para fins didáticos.

**Duração total:** 16 semanas
**Caminho crítico:** A1 → A2 → A4 → A5 → A6 → A7 → A9 → A10

| Cód. | Atividade | Dur. (sem) | Dep. | Folga (sem) | Crítico? |
|---|---|---|---|---|---|
| A1 | Levantamento de requisitos na oficina | 2 | — | 0 | Sim |
| A2 | Modelagem arquitetural e banco (PostgreSQL) | 2 | A1 | 0 | Sim |
| A3 | Configuração do ambiente e DevOps (Docker) | 1 | A2 | 1 | Não |
| A4 | Módulo de autenticação e segurança (JWT) | 1 | A2 | 0 | Sim |
| A5 | Domínio base: clientes e veículos | 2 | A4 | 0 | Sim |
| A6 | Domínio central: orçamentos e ordens de serviço | 3 | A5 | 0 | Sim |
| A7 | Módulo financeiro e faturamento em PDF | 2 | A6 | 0 | Sim |
| A8 | Painel executivo / dashboard de KPIs | 1 | A6 | 1 | Não |
| A9 | Testes de integração e homologação na oficina | 2 | A7 | 0 | Sim |
| A10 | Redação da monografia / artigo SBC | 2 | A9 | 0 | Sim |

## Decisão de Fast Tracking
Após o atraso simulado de 3 semanas (ver `04-cronograma.md`, seção de compressão), optou-se por executar a redação do artigo em paralelo com a homologação e suprimir o dashboard de KPIs (A8), que não é crítico.

## Realizado simulado
- A8 foi removida do escopo entregue.
- A9 teve +1 semana por falha de compatibilidade do ambiente de homologação com a oficina piloto (mitigação do risco de CEP).
- Término real simulado: semana 17.
