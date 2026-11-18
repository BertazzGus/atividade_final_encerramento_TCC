# 09 — Relatório de Status Final

> **Aviso:** dados simulados para fins didáticos. Data de referência: 17/11/2026.

## Farol por dimensão
| Dimensão | Linha de base | Realizado (simulado) | Farol |
|---|---|---|---|
| Escopo | 8 pacotes | 7 de 8 pacotes entregues (KPIs removidos); 87,5% | 🟡 |
| Prazo | 16 semanas | 17 semanas (+1 semana na homologação) | 🟡 |
| Custo | Linha de base R$ 28.847 | CR final R$ 26.520 (abaixo da linha de base) | 🟢 |
| Riscos | 7 riscos (6 registrados + R7 identificado) | R1 materializado e tratado; R7 não previsto | 🟡 |
| Qualidade | Isolamento, testes, SBC, reprodutibilidade | Isolamento verificado; defeitos críticos corrigidos; artigo aprovado após 2 revisões | 🟢 |

## Indicadores finais
| Indicador | Valor | Cálculo |
|---|---|---|
| Percentual de escopo entregue | 87,5% | 7 entregáveis ÷ 8 previstos × 100 |
| Desvio de prazo | +1 semana (+6,3%) | (17 − 16) / 16 |
| Horas planejadas (PERT) | 835,7 h | Tabela 1 do orçamento |
| Horas realizadas (simulado) | 854 h | Soma dos pacotes (ver tabela abaixo) |
| Desvio de horas | +2,2% | (854 − 835,7) / 835,7 |
| VA final | R$ 25.980 | Valor agregado das entregas aceitas |
| CR final (custo real) | R$ 26.520 | 854 h × R$ 30 + R$ 900 em custos diretos simulados |
| IDC final | 0,98 | VA / CR = 25.980 / 26.520 |
| IDP final | 0,90 | VA / VP = 25.980 / 28.847 |
| VC final | −R$ 540 | VA − CR |
| VPr final | −R$ 2.867 | VA − VP |

## Horas por pacote (PERT × realizado)
| Pacote | PERT (h) | Realizado (h) | Desvio (%) | Explicação |
|---|---|---|---|---|
| 1.1 Requisitos e contexto | 50,7 | 52 | +2,6 | Ajustes de requisitos após levantamento na oficina |
| 1.2 Arquitetura e dados | 50,0 | 49 | −2,0 | Sem desvio relevante |
| 1.3 Backend, autenticação e tenant | 168,3 | 185 | +9,9 | Refatoração do filtro de tenant após testes de acesso cruzado |
| 1.4 Fluxos operacionais e regras | 146,7 | 150 | +2,2 | Regras de faturamento mais complexas que o previsto |
| 1.5 Interface web e painéis | 188,3 | 170 | −9,7 | KPIs removidos (M1) |
| 1.6 Integração e implantação | 53,3 | 58 | +8,8 | Tratamento de erro do CEP (M2) |
| 1.7 Validação e ajustes | 73,3 | 80 | +9,1 | Homologação com a oficina piloto |
| 1.8 Artigo e defesa | 105,0 | 110 | +4,8 | Uma revisão adicional |
| **Total** | **835,7** | **854** | **+2,2** | |

**Três maiores desvios absolutos:** 1.5 (−18 h, compensado pela remoção do escopo), 1.3 (+17 h) e 1.7 (+7 h).

## Pendências entregues ao patrocinador
- Relatórios secundários (M3) não implementados; registrados como escopo cortado.
- Dashboard de KPIs (M1) não implementado; recomendado para versão futura.
- Validação com usuários reais da oficina restrita à oficina piloto.
