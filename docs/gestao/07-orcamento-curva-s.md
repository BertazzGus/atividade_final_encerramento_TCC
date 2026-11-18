# 07 — Orçamento e Curva S

> **Aviso:** dados simulados para fins didáticos. Não há apontamentos reais de horas nem comprovantes. Os valores de custo direto e a data de status são premissas.

## 1. Estimativa bottom-up (PERT)
Fórmulas: E = (O + 4M + P) / 6 e σ = (P − O) / 6. Custo de oportunidade: R$ 30/h.

| EAP | Pacote | O (h) | M (h) | P (h) | PERT (h) | σ | Custo (R$) |
|---|---|---|---|---|---|---|---|
| 1.1 | Requisitos e contexto | 32 | 48 | 80 | 50,7 | 8,0 | 1.520 |
| 1.2 | Arquitetura e dados | 30 | 48 | 78 | 50,0 | 8,0 | 1.500 |
| 1.3 | Backend, autenticação e tenant | 100 | 160 | 270 | 168,3 | 28,3 | 5.050 |
| 1.4 | Fluxos operacionais e regras | 80 | 140 | 240 | 146,7 | 26,7 | 4.400 |
| 1.5 | Interface web e painéis | 110 | 180 | 300 | 188,3 | 31,7 | 5.650 |
| 1.6 | Integração e implantação | 30 | 50 | 90 | 53,3 | 10,0 | 1.600 |
| 1.7 | Validação e ajustes | 40 | 70 | 120 | 73,3 | 13,3 | 2.200 |
| 1.8 | Artigo e defesa | 60 | 100 | 170 | 105,0 | 18,3 | 3.150 |
| | **Total** | **482** | **796** | **1.348** | **835,7** | **57,1** | **25.070** |

Desvio-padrão total: √(Σσ²) = 57,1 h (independência entre pacotes).

## 2. Outros custos diretos e indiretos
| Item | Natureza | Comportamento | Cálculo | R$ |
|---|---|---|---|---|
| Domínio | Direto | Fixo | 1 registro | 50 |
| Deslocamentos | Direto | Variável | Visitas à oficina | 80 |
| Impressão e encadernação | Direto | Variável | Provisão | 100 |
| Rateio de indiretos | Indireto | Variável | 10% × R$ 25.300 | 2.530 |
| **Total** | | | | **2.760** |

## 3. Reserva de contingência
| Risco | Prob. | Impacto (R$) | VME (R$) |
|---|---|---|---|
| Retrabalho após retorno da oficina | 35% | 900 | 315 |
| Menor disponibilidade por disciplinas/trabalho | 40% | 1.350 | 540 |
| Adaptação a falha/alteração de serviço externo | 20% | 360 | 72 |
| Perda local e recuperação de código | 10% | 900 | 90 |
| **Contingência** | | | **1.017** |

## 4. Orçamento
- Custos das estimativas + despesas diretas e indiretas: R$ 27.830
- Linha de base (+ contingência R$ 1.017): **R$ 28.847**
- Reserva gerencial (5% da linha de base): R$ 1.442,35
- **Orçamento total: R$ 30.289,35**

## 5. Curva S (linha de base distribuída por mês)
| Mês/2026 | Atividades principais | Mês (R$) | VP acumulado (R$) |
|---|---|---|---|
| Mar. | Requisitos e início da arquitetura | 2.596,23 | 2.596,23 |
| Abr. | Arquitetura e início do backend | 4.038,58 | 6.634,81 |
| Mai. | Backend e fluxos operacionais | 5.192,46 | 11.827,27 |
| Jun. | Backend, interface e integração | 5.480,93 | 17.308,20 |
| Jul. | Interface e integração | 4.615,52 | 21.923,72 |
| Ago. | Testes e homologação | 3.461,64 | 25.385,36 |
| Set. | Artigo e ajustes finais | 2.019,29 | 27.404,65 |
| Out. | Defesa e encerramento | 1.442,35 | 28.847,00 |

## 6. Valor agregado na data de status (30/06, mês 4) — simulado
| Indicador | Valor | Cálculo |
|---|---|---|
| ONT | R$ 28.847,00 | Linha de base |
| VP | R$ 17.308,20 | 60% da linha de base |
| VA | R$ 13.846,56 | 48% do orçamento em entregas aceitas |
| CR | R$ 14.750,00 | 480 h × R$ 30 + R$ 350 em custos diretos |
| VC | −R$ 903,44 | VA − CR |
| VPr | −R$ 3.461,64 | VA − VP |
| IDC | 0,94 | VA / CR |
| IDP | 0,80 | VA / VP |

**Diagnóstico:** IDC e IDP abaixo de 1 indicam custo acima do valor agregado e atraso.

## 7. Previsão de custo na data de status
- ENT típica = ONT / IDC = R$ 30.729,17
- ENT com atraso e baixa eficiência = CR + (ONT − VA) / (IDC × IDP) = R$ 34.723,96
- EPT = ENT − CR = R$ 15.979,17
- VNT = ONT − ENT = −R$ 1.882,17
- IDPT = (ONT − VA) / (ONT − CR) = 1,06

**Leitura:** se o atraso persistir junto com a baixa eficiência, a ENT com fórmula composta é mais prudente. Se o atraso for pontual, a ENT típica pode ser mais adequada.
