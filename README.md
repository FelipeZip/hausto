# Hausto

Agente que ajuda o cliente a decidir **quanto pagar da fatura do cartão** sem faltar dinheiro para as despesas essenciais. Projeto da Batalha de Agentes Itaú.

> Todos os dados são **fictícios** e as taxas são **ilustrativas**.

## Conteúdo

| Arquivo | O que é |
|---|---|
| [`app-mobile/index.html`](app-mobile/index.html) | Protótipo do app mobile com o Hausto (abra direto no navegador) |
| [`LEVANTAMENTO_DADOS_E_PERSONAS.md`](LEVANTAMENTO_DADOS_E_PERSONAS.md) | Análise da base (467 mil transações, 1.000 clientes fictícios, 2025) |
| [`Hausto_Personas.md`](Hausto_Personas.md) | Personas (INSS, CLT e PJ/MEI) e premissas de cálculo |
| [`Hausto_UX_Agente.md`](Hausto_UX_Agente.md) | Diretrizes de UX e conversa do agente |
| [`user_features_clustered.csv`](user_features_clustered.csv) | Features por cliente com o cluster atribuído |
| [`cluster_profiles.csv`](cluster_profiles.csv) | Perfil médio de cada cluster |
| `Hausto_Ficha_Submissao_Eleven.pptx` | Ficha de submissão |
| `Hausto_Posicionamento_Final_PF_Eleven_Atualizado.pptx` | Apresentação de posicionamento |

## Dados

A base bruta de transações (`bq-results-*.csv`, 63 MB) não está no repositório por causa do tamanho. As colunas estão descritas em `LEVANTAMENTO_DADOS_E_PERSONAS.md`.
