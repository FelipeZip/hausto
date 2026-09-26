# Hausto — UX do Agente

> Diretrizes de experiência para o Hausto, o agente que ajuda o cliente a decidir quanto pagar da fatura sem faltar dinheiro para as despesas essenciais.
> Público: em sua maioria, pessoas sem familiaridade com finanças, divididas em três perfis de renda (**INSS**, **sem vínculo** e **CLT**).

---

## 1. Ponto de partida

O tom importa, mas é só uma parte. Em um agente, **a conversa é a própria interface**. Por isso o trabalho de UX define:

- **o que** o Hausto fala;
- **em que ordem** ele fala;
- **em que formato** a informação aparece;
- **como ele se adapta** a cada perfil;
- **como ele confere** se a pessoa entendeu.

O tom é a última camada disso tudo.

---

## 2. As três perguntas que o UX de um agente responde

| Pergunta | No Hausto |
|---|---|
| **O que dizer, e quando?** | Uma decisão por mensagem. Mostrar primeiro a consequência e só depois o conceito. |
| **Como dizer?** | Em reais e em datas, sem jargão, sem julgamento e com botões de resposta. |
| **A pessoa entendeu?** | Pedir que ela diga com as palavras dela o que entendeu (*teach-back*), em vez de perguntar "entendeu?". |

---

## 3. Princípios para quem não entende de finanças

1. **Começar pela consequência, não pelo conceito.**
   Em vez de "juros rotativos de 13% a.m.", dizer algo como "se pagar só o mínimo, mês que vem a dívida quase não diminui".
2. **Usar como número principal o quanto sobra até a próxima renda.**
   É isso que a pessoa sente no dia a dia. O CET fica para quem pedir mais detalhes.
3. **Oferecer no máximo três caminhos, sempre com botões.**
   Texto livre só como opção extra, e sempre com a opção "não sei".
4. **Confirmar dados em vez de pedir.**
   "Vi que você gasta uns R$ 400 de mercado. Está certo? [Sim] [É mais] [É menos]" é muito mais fácil do que "informe suas despesas essenciais".
5. **Arredondar para explicar e ser exato para pagar.**
   "Uns R$ 480" na explicação e "R$ 478,93" só na hora de confirmar o pagamento.
6. **Não julgar.**
   Nunca usar "você está endividado" ou "você errou". Sempre fechar com "a decisão é sua".
7. **Mostrar o detalhe só quando pedirem.**
   Um botão "quer ver a conta completa?" atende quem sabe mais sem sobrecarregar quem sabe menos.
8. **Deixar claro que é seguro.**
   O agente se apresenta, nunca pede senha e nunca manda link. Isso é essencial para o público do INSS, que é muito visado por golpes.

### Glossário de tradução (termo → como o Hausto fala)

| Evitar | Usar |
|---|---|
| Juros rotativos | Juros cobrados quando você paga menos que o total |
| CET | Quanto isso vai custar no total |
| Saldo remanescente | O que fica faltando pagar |
| Amortização | Quanto a dívida diminui |
| Parcelamento da fatura | Dividir o que falta em parcelas (com juros) |
| Despesas essenciais | Contas que não dá para deixar de pagar: aluguel, luz, remédio, mercado |

---

## 4. Adaptação por perfil

O tom quase não muda entre os perfis. O que muda é **a pergunta sobre a renda** e **quanta margem de segurança a conta deixa**.

| | INSS | Sem vínculo | CLT |
|---|---|---|---|
| **Renda** | Fixa, com data conhecida pelo calendário do INSS | Irregular e incerta | Fixa, às vezes com adiantamento |
| **Pergunta-chave** | "Seu benefício cai dia 3, certo?" | "Até dia 10, quanto você acha que entra?" (por faixas) | "Você recebe adiantamento dia 20?" |
| **Como calcular** | Direto | **Usar o cenário mais baixo**, para não deixar a pessoa sem dinheiro | Direto, considerando 13º e férias |
| **Formato** | Mensagens curtas, fonte grande, opção de áudio, sem tabelas | Direto e prático | Pode ser mais enxuto |
| **Risco principal** | Golpe e consignado já descontado da renda | Superestimar o quanto vai entrar | Excesso de confiança ("o salário cobre") |

---

## 5. Exemplo de antes e depois

*Valores ilustrativos.*

### Antes

> Sua fatura de R$ 1.240,00 vence em 10/10. Pagamento mínimo: R$ 186,00. O saldo remanescente incorrerá em encargos rotativos (CET 380% a.a.).

### Depois (perfil INSS)

**Abertura:**

> Oi, Dona Maria. Sua fatura vence dia 10 e está em R$ 1.240.
> Seu benefício só cai dia 3, e até lá ainda tem aluguel, remédio e mercado.
> Separei 3 caminhos. Quer ver?
>
> **[Quero ver]** **[Agora não]**

**Comparação:**

> ✅ **Pagar R$ 600.** Sobram R$ 450, que dão para aluguel, remédio e mercado. Mês que vem ficam uns R$ 700 de dívida.
>
> ⚠️ **Pagar só o mínimo (R$ 186).** Sobra mais agora, mas mês que vem a dívida vira uns R$ 1.200 e quase não diminui.
>
> ❌ **Pagar tudo.** Faltam R$ 190 para o aluguel.

Os ícones sempre vêm acompanhados de texto, para não depender só de cor (acessibilidade).

**Checagem de compreensão (*teach-back*):**

> Só para conferir: se pagar só o mínimo, o que acontece com a dívida mês que vem?
>
> **[Diminui bastante]** **[Fica quase igual]** **[Some]**

Essa checagem mede diretamente a **métrica 3 (compreensão antes e depois da orientação)**.

### Perfil sem vínculo: pergunta sobre a renda

> Como sua renda muda de mês a mês, vou fazer a conta com um valor mais baixo para não te deixar na mão. Até dia 10, você acha que entra:
>
> **[Menos de R$ 800]** **[R$ 800 a 1.500]** **[Mais de R$ 1.500]** **[Não sei]**

---

## 6. Onde o UX entra na arquitetura

| Camada | Papel no UX |
|---|---|
| **BigQuery** | Fornece o histórico usado para *confirmar* dados (ex.: gasto médio com mercado) em vez de pedi-los do zero. |
| **Gemini + Google ADK (coleta)** | Faz as perguntas de acordo com o perfil (INSS, sem vínculo ou CLT). |
| **Funções no Cloud Run** | Calculam os cenários. **Todo número vem daqui**, em formato estruturado (cenários, sobra, dívida projetada). |
| **Gemini (explicação)** | **Não calcula, só redige.** Transforma os números em linguagem simples seguindo o guia de voz e tom. |

### Regras práticas

- **O Gemini não calcula nada.** Isso evita número inventado.
- **O guia de voz e tom vira regra no *system prompt*:**
  - frases com até cerca de 15 palavras;
  - lista de termos proibidos com as traduções correspondentes (ver glossário);
  - no máximo três opções por mensagem;
  - sempre mostrar quanto sobra até a próxima renda;
  - nunca pedir senha nem enviar link.
- **Um avaliador automático confere cada resposta contra esse guia.** Isso vira a **métrica 4 (% de respostas dentro dos limites definidos)**.
- **O perfil é uma variável do contexto** que muda as perguntas e a margem da conta, não a personalidade do agente.

---

## 7. O trabalho de UX na prática (ritmo de hackathon)

1. **Três proto-personas**, tiradas da base sintética:
   - Dona Maria, INSS, 67 anos;
   - Jonas, entregador, sem vínculo;
   - Carla, CLT, com adiantamento dia 20.
2. **Mapa da jornada da demo:** alerta → confirmação de dados → comparação → escolha → nova despesa essencial → recálculo e explicação.
3. **Roteiro da conversa** para cada persona, com o caminho feliz e dois ou três desvios:
   - "não sei";
   - "não concordo com o valor";
   - "quero pagar tudo mesmo assim".
4. **Guia de voz e tom**, que depois vira o *system prompt*.
5. **Teste com cinco pessoas reais**, de preferência pais, avós ou alguém do público do INSS. Uma pessoa da equipe faz o papel do agente pelo WhatsApp (teste *Wizard of Oz*), e o time mede quantos acertam a checagem de compreensão.
6. **Ajuste e repetição.** Um único teste já rende uma frase forte para o pitch, como "4 de 5 entenderam na primeira leitura".

---

## 8. Dica para a demo

Mostrar a **mesma fatura** conversada com Dona Maria e com Jonas lado a lado. Isso prova em poucos segundos que o agente se adapta à pessoa, e não só à conta.

---

## 9. Ligação com as métricas da ficha

| Métrica da ficha | Como o UX contribui |
|---|---|
| 1. Diferença de custo projetado entre opções | Cenários mostrados em reais e datas, com no máximo três caminhos. |
| 2. % de casos com o essencial preservado | "Quanto sobra até a próxima renda" como número principal, com cenário conservador para renda irregular. |
| 3. Compreensão antes e após a orientação | Checagem de compreensão (*teach-back*) com botões ao fim da comparação. |
| 4. % de respostas dentro dos limites definidos | Guia de voz e tom no *system prompt*, conferido por um avaliador automático. |
