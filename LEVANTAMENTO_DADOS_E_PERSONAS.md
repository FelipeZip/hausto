# Levantamento de Dados & Personas — Batalha de Agentes Itaú
### Base analisada: `bq-results-20260926-150302` · 467.585 transações · 1.000 clientes fictícios · ano de 2025 (jan–dez)

> Objetivo deste documento: reunir o levantamento de dados que embasa a **Ficha de Submissão – Parte 1** (Problema, Momento do Usuário, Dados & Tecnologia, Métricas, Personas). Todos os números vêm da análise real da base.

---

## 1. O que a base contém (e o que NÃO contém)

| Coluna | Significado |
|---|---|
| `id_usuario` | Identificador do cliente (1.000 únicos) |
| `anomesdia` / `anomes` | Data da transação (2025-01-01 a 2025-12-31) |
| `tipo` | `S` = saída/gasto (432.508) · `E` = entrada/receita (35.077) |
| `descr` | Descrição livre da transação |
| `vlr` | Valor em R$ |
| `nom_cate_macro` / `nom_cate_micro` | Categorização (25 macro-categorias) |
| `saldo_apos` | Saldo da conta após a transação |
| `parcela_atual` / `parcela_total` | Parcelamento (preenchido em 29.847 transações / 6,4%) |

⚠️ **Não há idade, gênero, CEP ou dado cadastral.** Personas e "perfil de usuário" são **inferidos do comportamento transacional** (renda, gasto, saldo, categorias, endividamento). Onde a ficha pede "idade e dados do usuário", entregamos **proxies comportamentais** (fase de vida inferida por: financiamento imobiliário, mensalidade escolar, pets, perfil de consumo).

---

## 2. Retrato financeiro geral (os 1.000 clientes)

- **Renda média:** R$ 8.441/mês · **Gasto médio:** R$ 8.467/mês → **na média, o cliente gasta tudo o que ganha** (taxa de poupança média **negativa**, −0,05).
- **Movimentação total no ano:** R$ 101,3 mi em entradas vs R$ 101,6 mi em saídas.
- **Salário identificado** em 800 clientes (salário médio ~R$ 5.000). Os outros 200 têm **renda informal/variável** (só "Recebimentos diversos").
- **Para onde o dinheiro vai (% do gasto total):**

| Categoria | % do gasto |
|---|---|
| Empréstimos e financiamentos | **24,6%** |
| Produtos financeiros (juros, tarifas, fatura) | **19,7%** |
| Casa (moradia, contas) | 14,1% |
| Educação | 7,8% |
| Lojas e sites | 4,7% |
| Lazer | 4,2% |
| Mercado + Restaurantes + Delivery | 7,1% |

👉 **Quase metade (44%) de todo o gasto é serviço da dívida e custo financeiro.** Este é o problema estrutural da base.

---

## 3. Problemas concretos detectados (evidências para a ficha)

| Problema | Nº de clientes | % da base |
|---|---:|---:|
| **Gastam mais do que ganham** (poupança negativa no ano) | **493** | 49,3% |
| **Sem reserva de emergência** (saldo médio < 1 mês de gasto) | 322 | 32,2% |
| **Ficaram com saldo negativo** em algum momento | 327 | 32,7% |
| **Comprometimento com dívida > 30% da renda** | 346 | 34,6% |
| **Fazem apostas/jogos** (bet, cassino, jogo digital) | 231 | 23,1% |
| **Não investem / não têm rendimentos** | 700 | 70,0% |

Notas de nuance:
- **Apostas** aparecem em 23% dos clientes, mas o valor é baixo (R$ 18,9 mil no ano todo, ~R$ 82/ano por apostador). É um **sinal comportamental/gatilho de alerta**, não a causa do endividamento.
- O vilão real é o **crédito caro + parcelamento**: 44% do gasto vira dívida/juros.

---

## 4. As 6 Personas (clusterização K-Means sobre comportamento)

> Segmentação feita com 19 variáveis (renda, gasto, poupança, saldo, dívida, categorias, investimento, parcelamento, filhos/imóvel). 6 grupos claros:

### 🔴 P1 — "Família no Vermelho" · 172 clientes (17%)
- Renda R$ 8,4 mil/mês, **gasta R$ 10,6 mil** → poupança **−26%**, saldo médio de só **R$ 1,2 mil**.
- **100% ficaram negativos**, dívida = 39% da renda. Todos têm imóvel financiado + filho na escola.
- **Dor:** ganha bem, mas o padrão de vida + financiamentos afundam a conta todo mês.

### 🔴 P2 — "Consumidor por Impulso" · 100 clientes (10%)
- Renda baixa (R$ 4,6 mil), **gasta R$ 7,5 mil** → poupança **−65%** (a pior).
- 73% ficam negativos; campeões de **delivery** (10% do gasto) e **assinaturas** (5,6 serviços/pessoa).
- **Dor:** consumo digital/impulso incompatível com a renda; sangria por pequenos gastos recorrentes.

### 🟠 P3 — "Classe Média no Aperto" · 232 clientes (23%) — *o maior grupo*
- Renda R$ 8,7 mil, gasto R$ 8,6 mil → **fica no zero a zero**. Dívida 31% da renda. **Não investe.**
- Paga tudo em dia mas **nunca sobra** para formar patrimônio.

### 🟢 P4 — "Família Investidora" · 296 clientes (30%) — *o maior grupo saudável*
- Renda R$ 11,4 mil, poupa **16,5%**, saldo médio **R$ 28 mil**. **100% investe**, casa + filhos.
- **Não é dor, é oportunidade:** cliente para engajamento/otimização, não resgate.

### 🟡 P5 — "Jovem sem Colchão" · 99 clientes (10%)
- Renda R$ 6,9 mil, quase sem dívida, mas **53% ficam negativos** e têm 3,7 assinaturas.
- Sem imóvel/filhos. **Dor:** vive no limite, qualquer imprevisto vira saldo negativo.

### 🟢 P6 — "Iniciante Baixa Renda" · 101 clientes (10%)
- Renda R$ 4,6 mil, mas **controlado** (poupa 6%, sem dívida). Gasta mais em lazer.
- **Dor leve:** renda baixa limita crescimento; candidato a educação financeira e primeiros investimentos.

---

## 5. Como isso preenche a Ficha (sugestão)

- **O Problema:** *"Metade dos clientes (49%) gasta mais do que ganha e 44% de todo o gasto vira dívida e juros."* Evidências: 327 ficaram negativos; 346 comprometem +30% da renda com dívida.
- **Momento do Usuário:** priorizar **P1 (Família no Vermelho)** e **P2 (Consumidor por Impulso)** — dor aguda e mensal, no momento em que o saldo cruza o vermelho.
- **Dados & Tecnologia:** transações categorizadas + saldo + parcelas → features de renda/gasto/poupança/dívida → clusterização + regras de alerta (saldo projetado, comprometimento de renda, gatilho de apostas).
- **Métricas de valor:** ① % de clientes que saem do vermelho; ② redução do comprometimento com dívida; ③ nº de clientes que passam a ter reserva ≥ 1 mês; ④ engajamento (P4/P6 começando a investir/poupar).
- **Escopo da Demo:** jornada de um cliente P1/P2 → agente detecta padrão de risco → gera diagnóstico + plano de ação personalizado.

---

*Artefatos gerados: `user_features_clustered.csv` (features + persona por cliente) e `cluster_profiles.csv` (perfil de cada persona) na pasta de trabalho.*
