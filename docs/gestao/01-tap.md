# 01 — Termo de Abertura do Projeto (TAP)

> **Aviso:** dados simulados para fins didáticos. Não há registros reais de horas ou despesas.

**Projeto:** MyMechanic — sistema web para gestão de oficinas mecânicas (TCC)
**Gerente e desenvolvedor:** Gustavo Bertuzzi de Oliveira
**Patrocinador / orientador:** Prof. Nelson Bellincanta Filho
**Stack:** Java 21, Spring Boot, Vue.js 3, PostgreSQL, arquitetura multi-tenant
**Duração planejada:** 16 semanas (caminho crítico)
**Orçamento (linha de base):** R$ 28.847,00 · Orçamento total com reserva gerencial: R$ 30.289,35

## 1. Objetivo e justificativa
Desenvolver um sistema web que centralize, em uma única solução, o cadastro de clientes, veículos, funcionários, peças e serviços, o controle de estoque, a elaboração de orçamentos, o acompanhamento de ordens de serviço, a emissão de faturas e a geração de relatórios para oficinas mecânicas, com isolamento de dados entre oficinas.

## 2. Escopo
**Incluído**
- Cadastros (clientes, veículos, funcionários, peças e serviços)
- Controle de estoque
- Orçamentos e ordens de serviço
- Faturamento com geração de PDF
- Relatórios gerenciais
- Isolamento multi-tenant
- Testes de integração e homologação na oficina piloto

**Excluído**
- Editor visual de faturas (ver decisão de trade-off no artigo)
- Cobertura de testes E2E com Cypress na interface (risco aceito)

## 3. Restrições
- Desenvolvimento individual
- 20 horas semanais disponíveis, além das reuniões com o orientador
- Prazo acadêmico inegociável para a defesa

## 4. Premissas
- Ferramentas e infraestrutura são open-source ou de execução local (Docker, PostgreSQL)
- A oficina piloto de Cascavel-PR está disponível para homologação
- O orientador validará as entregas nos marcos

## 5. Riscos principais
Ver registro completo no arquivo `05-riscos.md`. Destacam-se sobrecarga de tempo, retrabalho após qualificação e falha de isolamento multi-tenant.

## 6. Stakeholders
| Parte interessada | Papel |
|---|---|
| Gustavo Bertuzzi | Gerente e desenvolvedor |
| Prof. Nelson Bellincanta Filho | Orientador e patrocinador |
| Banca examinadora | Avaliação do TCC |
| Coordenação do curso | Prazos e documentos |
| Usuários de oficinas | Validação de fluxos e telas |

## 7. Critérios de sucesso
- Isolamento de dados entre tenants verificado por testes
- Entrega funcional dos módulos de cadastro, orçamentos, ordens de serviço, estoque e faturamento
- Relatórios gerenciais operacionais
- Conclusão dentro do prazo acadêmico, com defesa realizada
