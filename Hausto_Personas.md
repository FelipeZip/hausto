# Hausto — Personas

> Três personas para guiar o design da conversa, a base sintética e a demo do Hausto.
> Todos os dados são **fictícios** e as taxas são **ilustrativas**. Os números aqui substituem os exemplos soltos do arquivo `Hausto_UX_Agente.md`.

| | Persona | Perfil | Renda | Desafio central |
|---|---|---|---|---|
| 1 | **Dona Maria Aparecida** | INSS | Fixa, com consignado descontado | Está presa no ciclo do mínimo e tem medo de golpe |
| 2 | **Carla Menezes** | CLT | Fixa, dividida em salário e adiantamento | Acha que "o salário cobre", mas o dinheiro some antes do dia 20 |
| 3 | **Jonas Ferreira** | PJ (MEI) | Irregular, por serviço | Não sabe quanto vai entrar e mistura contas da empresa com as pessoais |

---

## Premissas de cálculo (valem para as três)

| Item | Valor usado |
|---|---|
| Juros do rotativo | **12% ao mês** (ilustrativo, sem IOF) |
| Juros do parcelamento da fatura | **8% ao mês** (ilustrativo, sem IOF) |
| Pagamento mínimo | **15%** da fatura |
| Dívida projetada | Saldo que ficou × 1,12, **sem contar compras novas** |
| Pagamento extra antes do próximo vencimento | Juros proporcionais aos dias (mês de 30 dias) |
| Folga | Saldo + entradas certas − pagamento da fatura − despesas essenciais até a próxima renda |
| Pagamento sugerido | Maior valor que ainda deixa as essenciais pagas e uma reserva mínima |

**Regras reais que a função de cálculo precisa respeitar:**
- O rotativo só pode ser usado até o vencimento seguinte. Depois disso, o banco precisa oferecer parcelamento (Resolução CMN 4.549/2017).
- Os juros e encargos do rotativo e do parcelamento não podem passar de 100% do valor original da dívida (Lei 14.690/2023).
- Pagar menos que o mínimo conta como atraso. Por isso, **o Hausto nunca sugere um valor abaixo do mínimo**.
- A demo **só compara** as opções. O Hausto não faz pagamento nem contrata parcelamento.

---

## Persona 1 — Dona Maria Aparecida dos Santos (INSS)

> *"Eu pago o que dá. Todo mês parece que a fatura é a mesma."*

### Quem é

| Campo | Dado |
|---|---|
| Idade | 67 anos |
| Cidade | Guarulhos (SP), periferia |
| Escolaridade | Ensino fundamental incompleto |
| Ocupação anterior | Costureira; hoje aposentada por idade |
| Moradia | Casa alugada, dividida com o neto |
| Família | Mora com o neto Kauã, de 19 anos, que faz bicos e divide o aluguel. É viúva e tem dois filhos que moram em outras cidades |
| Saúde | Hipertensa e diabética, com remédio de uso contínuo |

### Comportamento e tecnologia

| Campo | Dado |
|---|---|
| Letramento financeiro | **Baixo.** Não sabe o que é rotativo e confunde "mínimo" com "o que precisa pagar" |
| Letramento digital | **Baixo.** Usa WhatsApp e manda áudio. O neto a ajuda com o app do banco |
| Dispositivo | Android de entrada, tela pequena, fonte aumentada |
| Canal preferido | WhatsApp, com **áudio** |
| Horário de uso | Manhã (8h às 11h) |
| Confiança | Desconfia de mensagens do banco por medo de golpe. Já recebeu uma ligação falsa do "INSS" |
| Como decide | Pergunta ao neto ou à filha por telefone |

### Renda

| Item | Valor |
|---|---|
| Benefício bruto | R$ 2.050 |
| Consignado (desconto direto no benefício) | − R$ 530 |
| **Benefício líquido** | **R$ 1.520** |
| Dia em que o benefício cai | No início do mês, pelo calendário do INSS. Em outubro caiu dia 02; em novembro cai **dia 03** |

### Despesas essenciais do mês

| Despesa | Valor | Observação |
|---|---|---|
| Aluguel (parte dela) | R$ 470 | O aluguel total é R$ 900 e o neto paga o resto. **Já pago em outubro** |
| Mercado (dinheiro/Pix) | R$ 280 | Outra parte do mercado vai no cartão |
| Remédios | R$ 110 | Parte deles sai pela Farmácia Popular |
| Luz | R$ 90 | |
| Gás (metade) | R$ 55 | |
| Água | R$ 45 | |
| **Total** | **R$ 1.050** | |

### Cartão de crédito

| Campo | Dado |
|---|---|
| Limite | R$ 1.800 |
| Fatura atual | **R$ 1.240** |
| Mínimo | R$ 186 |
| Vencimento | **10/10** |

**Composição da fatura:**

| Item | Valor |
|---|---|
| Saldo do mês anterior, com juros | R$ 410 |
| Mercado | R$ 320 |
| Parcela da geladeira (3 de 6) | R$ 210 |
| Farmácia | R$ 180 |
| Parcela do celular do neto (5 de 10) | R$ 120 |
| **Total** | **R$ 1.240** |

### Histórico de 2025 (12 faturas)

| Tipo de pagamento | Quantidade | Quando |
|---|---|---|
| Total | 4 | Fevereiro, maio, agosto e dezembro (meses em que recebeu ajuda dos filhos ou o 13º) |
| Parcial | 3 | Janeiro, março e abril |
| Mínimo | 5 | Junho, julho, setembro, outubro e novembro |
| **Parcial ou mínimo** | **8 de 12** | É um padrão recorrente |

### O momento da decisão (06/10)

| Item | Valor |
|---|---|
| Saldo em conta hoje | **R$ 1.050** (R$ 1.520 do benefício menos R$ 470 do aluguel) |
| Próxima renda | 03/11, com R$ 1.520 |
| Essenciais até 03/11 | R$ 580 (mercado 280, remédio 110, luz 90, gás 55, água 45) |
| Reserva mínima | R$ 50 |
| **Pagamento sugerido** | **R$ 420** (1.050 − 580 − 50) |

### Cenários

| Opção | Paga agora | Folga até 03/11 | Dívida projetada no mês que vem | Juros no mês |
|---|---|---|---|---|
| Pagar tudo | R$ 1.240 | ❌ **faltam R$ 770** | R$ 0 | R$ 0 |
| **Pagar o sugerido** | **R$ 420** | ✅ **R$ 50** | ≈ R$ 918 | ≈ R$ 98 |
| Pagar só o mínimo | R$ 186 | ✅ R$ 284 | ≈ R$ 1.180 | ≈ R$ 126 |
| Parcelar o restante (apenas comparação) | R$ 186 + 6× R$ 228 | ✅ R$ 284 agora, mas as parcelas de R$ 228 comprometem os próximos 6 meses | — | Custo total ≈ R$ 314 |

### Evento da demo: nova despesa essencial

> "O médico passou um remédio novo, de R$ 90 por mês."

| | Antes | Depois |
|---|---|---|
| Essenciais até 03/11 | R$ 580 | R$ 670 |
| Pagamento sugerido | R$ 420 | **R$ 330** |
| Folga | R$ 50 | R$ 50 |
| Dívida projetada | ≈ R$ 918 | **≈ R$ 1.019** |

### Objetivos, dores e medos

- **Quer:** sair da fatura que "nunca acaba" e não depender do neto para entender o banco.
- **Dores:** o consignado já come parte do benefício, e a fatura não diminui mesmo pagando todo mês.
- **Medos:** cair em golpe, ficar sem remédio e ter o nome sujo.

### Como o Hausto se adapta a ela

- Trata por "senhora" e se apresenta toda vez: "Sou o Hausto, assistente do seu banco."
- Mensagens curtas, **sem tabelas** e com a opção **"ouvir em áudio"**.
- Usa a data do benefício como referência: "até o seu benefício cair, dia 3".
- Confirma os valores das contas em vez de perguntar: "O remédio fica em uns R$ 110 por mês, certo?"
- Sugere, de forma leve, que ela mostre a conversa para alguém de confiança, se quiser.

### Trecho de conversa

> **Hausto:** Bom dia, Dona Maria. Aqui é o Hausto, do seu banco.
> Sua fatura vence dia 10 e está em R$ 1.240. Seu benefício só cai dia 3 de novembro.
> Quer ajuda para ver quanto dá para pagar sem faltar para as contas da casa?
> **[Quero] [Ouvir em áudio] [Agora não]**

> **Hausto:** Até dia 3, a senhora ainda tem mercado, remédio, luz, gás e água. Dá uns R$ 580. Está certo?
> **[Está certo] [É mais] [É menos]**

> **Hausto:** Separei 3 caminhos:
> ✅ **Pagar R$ 420.** Todas as contas ficam pagas. Mês que vem a dívida fica em uns R$ 920.
> ⚠️ **Pagar só o mínimo (R$ 186).** Sobra mais agora, mas mês que vem a dívida fica em uns R$ 1.180, quase igual.
> ❌ **Pagar tudo.** Faltam R$ 770 para as contas do mês.
> A decisão é da senhora.

**Checagem de compreensão:**
> Só para conferir: pagando só o mínimo, o que acontece com a dívida mês que vem?
> **[Diminui bastante] [Fica quase igual] [Some]**

---

## Persona 2 — Carla Menezes (CLT)

> *"Quando o salário cai eu acho que dá pra tudo. No dia 15 já tô no vermelho."*

### Quem é

| Campo | Dado |
|---|---|
| Idade | 34 anos |
| Cidade | Recife (PE) |
| Escolaridade | Ensino médio completo |
| Ocupação | Auxiliar administrativa em uma rede de farmácias, com carteira assinada |
| Moradia | Apartamento alugado |
| Família | Mãe solo do Davi, de 8 anos, que estuda em escola pública |

### Comportamento e tecnologia

| Campo | Dado |
|---|---|
| Letramento financeiro | **Médio-baixo.** Sabe que o rotativo é caro, mas não sabe quanto, e não entende que pagar antes reduz os juros |
| Letramento digital | **Médio.** Usa bem o app do banco, Pix e compras online |
| Dispositivo | Android intermediário |
| Canal preferido | App do banco (notificação) e WhatsApp |
| Horário de uso | Na hora do almoço e à noite, depois que o filho dorme |
| Confiança | Confia no banco, mas ignora a maioria das notificações |
| Como decide | Rápido e sozinha, na hora de pagar |

### Renda

| Item | Valor | Data |
|---|---|---|
| Salário (líquido) | R$ 1.500 | 5º dia útil (em outubro, **07/10**) |
| Adiantamento (líquido) | R$ 1.000 | **Dia 20** |
| **Total líquido no mês** | **R$ 2.500** | |
| Vale-alimentação (cartão separado) | R$ 450 | Não entra na conta corrente |
| Vale-transporte | Descontado em folha | Cobre a ida ao trabalho |
| Extras no ano | 13º (novembro e dezembro) e 1/3 de férias (julho) | |

### Despesas essenciais do mês

| Despesa | Valor | Vencimento |
|---|---|---|
| Aluguel | R$ 800 | Dia 10 |
| Mercado complementar (além do VA) | R$ 270 | Ao longo do mês |
| Luz | R$ 130 | Dia 15 |
| Gás | R$ 120 | Por volta do dia 25 |
| Celular e internet | R$ 100 | Dia 12 |
| Farmácia e material escolar | R$ 100 | Ao longo do mês |
| Outros essenciais | R$ 80 | |
| **Total** | **R$ 1.600** | |

### Cartão de crédito

| Campo | Dado |
|---|---|
| Limite | R$ 3.000 |
| Fatura atual | **R$ 1.980** |
| Mínimo | R$ 297 |
| Vencimento | **12/10** |

**Composição da fatura:**

| Item | Valor |
|---|---|
| Saldo do mês anterior, com juros | R$ 460 |
| Mercado | R$ 350 |
| Roupas para a escola do filho | R$ 240 |
| Parcela da TV (6 de 10) | R$ 190 |
| Delivery | R$ 180 |
| Outros | R$ 160 |
| Parcela do celular (8 de 12) | R$ 150 |
| Transporte por aplicativo | R$ 120 |
| Farmácia | R$ 90 |
| Streaming | R$ 40 |
| **Total** | **R$ 1.980** |

### Histórico de 2025 (12 faturas)

| Tipo de pagamento | Quantidade | Quando |
|---|---|---|
| Total | 6 | Em geral nos meses sem gasto extra, e em dezembro (13º) |
| Parcial | 5 | Janeiro e março (material escolar), julho (férias do filho), setembro e outubro |
| Mínimo | 1 | Fevereiro |
| **Parcial ou mínimo** | **6 de 12** | Acontece nos meses com gasto sazonal |

### O momento da decisão (07/10, dia em que o salário caiu)

| Item | Valor |
|---|---|
| Saldo em conta hoje | **R$ 1.620** (R$ 1.500 do salário mais R$ 120 que sobraram) |
| Próxima renda | 20/10, com o adiantamento de R$ 1.000 |
| Essenciais até 20/10 | R$ 1.200 (aluguel 800, luz 130, celular e internet 100, mercado 120, farmácia e escola 50) |
| Essenciais de 20/10 até o próximo salário (06/11) | R$ 400 (mercado 150, gás 120, outros 80, farmácia e escola 50) |
| Reserva mínima | R$ 50 |
| **Pagamento sugerido agora** | **R$ 370** (1.620 − 1.200 − 50) |
| **Pagamento extra possível no dia 20** | **R$ 550** (1.000 − 400 − 50) |

### Cenários

| Opção | Paga agora | Folga até 20/10 | Dívida projetada no mês que vem | Juros no mês |
|---|---|---|---|---|
| Pagar tudo | R$ 1.980 | ❌ **faltam R$ 1.560** | R$ 0 | R$ 0 |
| Pagar só o mínimo | R$ 297 | ✅ R$ 123 | ≈ R$ 1.885 | ≈ R$ 202 |
| Pagar o sugerido | R$ 370 | ✅ R$ 50 | ≈ R$ 1.803 | ≈ R$ 193 |
| **Sugerido + R$ 550 no dia 20** | **R$ 370 + R$ 550** | ✅ **R$ 50** | **≈ R$ 1.205** | **≈ R$ 145** |
| Parcelar o restante (apenas comparação) | R$ 297 + 10× R$ 251 | ✅ R$ 123 agora, mas as parcelas comprometem 10 meses | — | Custo total ≈ R$ 827 |

> **O ponto que a Carla não sabe:** ela pode pagar uma parte agora e **mais uma parte no dia 20**, quando cai o adiantamento. Os juros correm por dia, então pagar antes do próximo vencimento reduz o custo.

### Evento da demo: nova despesa essencial

> "A geladeira quebrou e o conserto custa R$ 70."

| | Antes | Depois |
|---|---|---|
| Essenciais até 20/10 | R$ 1.200 | R$ 1.270 |
| Pagamento sugerido agora | R$ 370 | **R$ 297 (o mínimo)** |
| Folga até 20/10 | R$ 50 | R$ 53 |
| Pagamento extra no dia 20 | R$ 550 | R$ 550 |
| Dívida projetada | ≈ R$ 1.205 | **≈ R$ 1.287** |

### Objetivos, dores e medos

- **Quer:** parar de "começar o mês devendo" e conseguir dar o que o filho precisa.
- **Dores:** gastos pequenos no cartão (delivery, aplicativo) que somam muito, e a fatura que chega junto com o aluguel.
- **Medos:** não ter dinheiro se o filho ficar doente e perder o controle do cartão.

### Como o Hausto se adapta a ela

- Mensagens mais enxutas, direto ao ponto, com números lado a lado.
- Usa **as duas datas de renda** (salário e dia 20) e **propõe o pagamento em duas partes**.
- Quebra o excesso de confiança com fatos: "Depois do aluguel e das contas, sobram R$ 420 até o dia 20."
- Pode oferecer um lembrete no dia 20 para o pagamento extra.

### Trecho de conversa

> **Hausto:** Oi, Carla. Seu salário caiu hoje e a fatura de R$ 1.980 vence dia 12.
> Até o adiantamento do dia 20 você ainda tem aluguel, luz, celular e mercado, uns R$ 1.200.
> Quer ver quanto dá para pagar sem apertar?
> **[Quero ver] [Agora não]**

> **Hausto:** Uma ideia que ajuda: pagar em duas vezes.
> ✅ **R$ 370 agora + R$ 550 no dia 20.** Mês que vem a dívida cai para uns R$ 1.200.
> ⚠️ **Só o mínimo (R$ 297).** Mês que vem a dívida fica em uns R$ 1.890.
> ❌ **Pagar tudo agora.** Faltam R$ 1.560 para as contas até o dia 20.
> Quer que eu te lembre no dia 20? **[Sim, me lembra] [Não precisa]**

**Checagem de compreensão:**
> Pra conferir: por que pagar R$ 550 no dia 20 ajuda, se a fatura já venceu?
> **[Os juros diminuem] [Não muda nada] [Tira o nome do Serasa]**

---

## Persona 3 — Jonas Ferreira (PJ / MEI)

> *"Tem mês que entra bem, tem mês que não entra nada. O cartão segura as pontas."*

### Quem é

| Campo | Dado |
|---|---|
| Idade | 31 anos |
| Cidade | Belo Horizonte (MG) |
| Escolaridade | Ensino médio completo e curso técnico em refrigeração |
| Ocupação | Técnico de instalação e manutenção de ar-condicionado, **MEI** |
| Moradia | Casa alugada, dividida com a companheira |
| Família | Mora com a companheira Bruna, que é CLT. Tem uma filha de 6 anos de outro relacionamento, para quem paga pensão |
| Ferramenta de trabalho | Carro próprio (Fiat Strada 2014) |

### Comportamento e tecnologia

| Campo | Dado |
|---|---|
| Letramento financeiro | **Baixo a médio.** Sabe fazer orçamento de serviço, mas não separa o dinheiro da empresa do pessoal |
| Letramento digital | **Médio-alto.** Recebe por Pix, emite nota pelo app do MEI e usa WhatsApp Business |
| Dispositivo | Android intermediário, sempre no bolso durante o serviço |
| Canal preferido | WhatsApp, com mensagens rápidas entre um serviço e outro |
| Horário de uso | Irregular. Costuma olhar à noite |
| Confiança | Confia no banco, mas não tem paciência para textos longos |
| Como decide | Olha o saldo e "vai levando" |

### Renda (irregular)

| Mês (2026) | Faturamento líquido |
|---|---|
| Abril | R$ 2.300 |
| Maio | R$ 1.900 |
| Junho | R$ 1.600 |
| Julho | R$ 1.800 |
| Agosto | R$ 2.700 |
| Setembro | R$ 3.400 |
| **Média dos 6 meses** | **≈ R$ 2.283** |
| **Pior mês** | **R$ 1.600** |

**Sazonalidade:** a demanda é alta no verão (dezembro a março, com meses acima de R$ 4.000) e baixa no inverno (junho e julho).

**Serviços já agendados no momento da decisão:**

| Data | Serviço | Valor | Status |
|---|---|---|---|
| 22/10 | Instalação | R$ 600 | ✅ Confirmado |
| 28/10 | Manutenção | R$ 350 | ⏳ A confirmar |

### Despesas essenciais do mês

| Despesa | Valor | Vencimento | Tipo |
|---|---|---|---|
| Aluguel (metade) | R$ 750 | Dia 05 | Pessoal |
| Mercado | R$ 450 | Ao longo do mês | Pessoal |
| Pensão alimentícia | R$ 400 | Dia 05 | Pessoal, **inegociável** |
| Combustível e material | R$ 350 | Por serviço | Trabalho |
| Luz (metade) | R$ 90 | Dia 15 | Pessoal |
| DAS do MEI | R$ 86 (ilustrativo) | Dia 20 | Trabalho |
| Internet (metade) | R$ 60 | Dia 10 | Pessoal |
| **Total** | **R$ 2.186** | | |

### Cartão de crédito

| Campo | Dado |
|---|---|
| Limite | R$ 4.500 |
| Fatura atual | **R$ 2.760** |
| Mínimo | R$ 414 |
| Vencimento | **18/10** |

**Composição da fatura (mistura trabalho e vida pessoal):**

| Item | Valor | Tipo |
|---|---|---|
| Material de trabalho (tubos de cobre, gás refrigerante) | R$ 980 | Trabalho |
| Saldo do mês anterior, com juros | R$ 540 | — |
| Combustível | R$ 420 | Trabalho |
| Mercado | R$ 380 | Pessoal |
| Lanches e restaurante | R$ 210 | Misto |
| Parcela da bomba de vácuo (4 de 8) | R$ 170 | Trabalho |
| Plano de celular | R$ 60 | Misto |
| **Total** | **R$ 2.760** | |

### Histórico de 2025 (12 faturas)

| Tipo de pagamento | Quantidade | Quando |
|---|---|---|
| Total | 5 | Dezembro a março (verão) e setembro |
| Parcial | 4 | Abril, maio, agosto e outubro |
| Mínimo | 3 | Junho, julho e novembro |
| **Parcial ou mínimo** | **7 de 12** | Acompanha a sazonalidade do trabalho |

### O momento da decisão (15/10)

| Item | Valor |
|---|---|
| Saldo em conta hoje (pessoal e MEI juntos) | **R$ 2.200** |
| Entradas certas até 05/11 | R$ 600 (22/10) |
| Entradas prováveis até 05/11 | + R$ 350 (28/10, a confirmar) |
| Essenciais até 05/11 | R$ 1.966 (aluguel 750, pensão 400, mercado 330, combustível e material 250, luz 90, DAS 86, internet 60) |
| Reserva mínima | **R$ 150** (maior que a dos outros perfis, porque a renda é incerta) |
| **Pagamento sugerido (só com o que é certo)** | **R$ 680** (2.200 + 600 − 1.966 − 150 ≈ 684) |
| **Pagamento extra, se o serviço do dia 28 confirmar** | **R$ 350** |

### Cenários

Os cenários usam só a renda certa. O serviço do dia 28 só entra se for confirmado.

| Opção | Paga agora | Folga até 05/11 | Dívida projetada no mês que vem | Juros no mês |
|---|---|---|---|---|
| Pagar tudo | R$ 2.760 | ❌ **faltam R$ 1.926** | R$ 0 | R$ 0 |
| Pagar só o mínimo | R$ 414 | ✅ R$ 420 | ≈ R$ 2.628 | ≈ R$ 282 |
| **Pagar o sugerido** | **R$ 680** | ✅ **R$ 154** | ≈ R$ 2.330 | ≈ R$ 250 |
| Sugerido + R$ 350 no dia 28 (se confirmar) | R$ 680 + R$ 350 | ✅ R$ 154 | **≈ R$ 1.952** | ≈ R$ 222 |
| Parcelar o restante (apenas comparação) | R$ 414 + 12× R$ 311 | ✅ R$ 420 agora, mas as parcelas comprometem 12 meses, inclusive o inverno | — | Custo total ≈ R$ 1.390 |

> **O ponto que o Jonas não sabe:** fazer a conta com o dinheiro que **ainda não entrou** é o que o leva ao mínimo. O Hausto calcula com o que é certo e trata o resto como bônus.

### Evento da demo: nova despesa essencial

> "O pneu do carro furou e a troca custa R$ 220. Sem o carro eu não trabalho."

| | Antes | Depois |
|---|---|---|
| Essenciais até 05/11 | R$ 1.966 | R$ 2.186 |
| Pagamento sugerido | R$ 680 | **R$ 460** |
| Folga até 05/11 | R$ 154 | R$ 154 |
| Dívida projetada | ≈ R$ 2.330 | **≈ R$ 2.576** |

### Objetivos, dores e medos

- **Quer:** atravessar o inverno sem se afundar no cartão e comprar um carro melhor para trabalhar.
- **Dores:** não sabe quanto vai ganhar, paga material no cartão pessoal e o DAS às vezes atrasa.
- **Medos:** ficar sem carro (e sem trabalho), atrasar a pensão e perder o CNPJ.

### Como o Hausto se adapta a ele

- Mensagens **bem curtas**, que dá para ler entre um serviço e outro.
- Pergunta sobre a renda **por faixas** e separa o que é **certo** do que é **provável**.
- Faz a conta com o **cenário mais baixo** e deixa uma reserva maior.
- Trata como essenciais as despesas de trabalho (combustível, material, DAS) e a pensão.
- Pode avisar quando o serviço do dia 28 entrar, para ele decidir se paga o extra.

### Trecho de conversa

> **Hausto:** Fala, Jonas. Sua fatura de R$ 2.760 vence dia 18.
> Até dia 5 de novembro você tem aluguel, pensão, mercado, DAS e combustível, uns R$ 1.970.
> Quanto você tem de serviço **certo** até lá?
> **[Até R$ 500] [R$ 500 a 1.000] [Mais de R$ 1.000] [Não sei]**

> **Hausto:** Vou contar só com os R$ 600 do dia 22, que estão confirmados. Os R$ 350 do dia 28 ficam como bônus.
> ✅ **Pagar R$ 680.** Todas as contas ficam pagas e sobra uma reserva.
> ➕ Se o serviço do dia 28 entrar, pagar mais R$ 350 derruba a dívida para uns R$ 1.950.
> ⚠️ **Só o mínimo (R$ 414).** Mês que vem a dívida fica em uns R$ 2.630.
> ❌ **Pagar tudo.** Faltam R$ 1.926 para as contas.
> Quer que eu te avise quando o Pix do dia 28 cair? **[Quero] [Não precisa]**

**Checagem de compreensão:**
> Pra conferir: por que eu não contei os R$ 350 do dia 28?
> **[Porque ainda não é certo] [Porque é pouco] [Esqueci]**

---

## Comparativo das três personas

| | Dona Maria (INSS) | Carla (CLT) | Jonas (PJ/MEI) |
|---|---|---|---|
| Renda líquida | R$ 1.520 fixa | R$ 2.500 fixa, em 2 partes | ≈ R$ 2.283 de média, pior mês R$ 1.600 |
| Fatura | R$ 1.240 | R$ 1.980 | R$ 2.760 |
| Mínimo | R$ 186 | R$ 297 | R$ 414 |
| Parcial ou mínimo em 2025 | 8 de 12 | 6 de 12 | 7 de 12 |
| Pagamento sugerido | R$ 420 | R$ 370 + R$ 550 no dia 20 | R$ 680 + R$ 350 se confirmar |
| Reserva mínima | R$ 50 | R$ 50 | R$ 150 |
| Letramento financeiro | Baixo | Médio-baixo | Baixo a médio |
| Letramento digital | Baixo | Médio | Médio-alto |
| Canal | WhatsApp com áudio | App e WhatsApp | WhatsApp, mensagens curtas |
| Tom | Acolhedor e respeitoso, trata por "senhora" | Direto e prático | Bem curto e informal |
| Principal aprendizado | O mínimo não diminui a dívida | Pagar em duas vezes reduz os juros | Fazer a conta só com o que é certo |
| Evento da demo | Remédio novo (+R$ 90) | Conserto da geladeira (+R$ 70) | Pneu do carro (+R$ 220) |

---

## Dados para a base sintética

Formato sugerido para carregar as personas nos testes das funções do Cloud Run.

```json
[
  {
    "persona_id": "P01_INSS",
    "nome": "Maria Aparecida dos Santos",
    "idade": 67,
    "perfil_renda": "INSS",
    "cidade": "Guarulhos-SP",
    "letramento_financeiro": "baixo",
    "letramento_digital": "baixo",
    "canal": "whatsapp_audio",
    "renda": [
      { "descricao": "beneficio_liquido", "valor": 1520.00, "data": "2026-11-03", "certeza": "certa" }
    ],
    "descontos_em_folha": [{ "descricao": "consignado", "valor": 530.00 }],
    "data_decisao": "2026-10-06",
    "saldo_conta": 1050.00,
    "fatura": { "valor": 1240.00, "minimo": 186.00, "vencimento": "2026-10-10", "limite": 1800.00 },
    "essenciais_ate_proxima_renda": [
      { "descricao": "mercado", "valor": 280.00 },
      { "descricao": "remedios", "valor": 110.00 },
      { "descricao": "luz", "valor": 90.00 },
      { "descricao": "gas", "valor": 55.00 },
      { "descricao": "agua", "valor": 45.00 }
    ],
    "reserva_minima": 50.00,
    "historico_2025": { "total": 4, "parcial": 3, "minimo": 5 },
    "evento_demo": { "descricao": "remedio_novo", "valor": 90.00 }
  },
  {
    "persona_id": "P02_CLT",
    "nome": "Carla Menezes",
    "idade": 34,
    "perfil_renda": "CLT",
    "cidade": "Recife-PE",
    "letramento_financeiro": "medio_baixo",
    "letramento_digital": "medio",
    "canal": "app_whatsapp",
    "renda": [
      { "descricao": "adiantamento", "valor": 1000.00, "data": "2026-10-20", "certeza": "certa" },
      { "descricao": "salario", "valor": 1500.00, "data": "2026-11-06", "certeza": "certa" }
    ],
    "data_decisao": "2026-10-07",
    "saldo_conta": 1620.00,
    "fatura": { "valor": 1980.00, "minimo": 297.00, "vencimento": "2026-10-12", "limite": 3000.00 },
    "essenciais_ate_proxima_renda": [
      { "descricao": "aluguel", "valor": 800.00 },
      { "descricao": "luz", "valor": 130.00 },
      { "descricao": "celular_internet", "valor": 100.00 },
      { "descricao": "mercado", "valor": 120.00 },
      { "descricao": "farmacia_escola", "valor": 50.00 }
    ],
    "essenciais_entre_adiantamento_e_salario": 400.00,
    "reserva_minima": 50.00,
    "historico_2025": { "total": 6, "parcial": 5, "minimo": 1 },
    "evento_demo": { "descricao": "conserto_geladeira", "valor": 70.00 }
  },
  {
    "persona_id": "P03_PJ",
    "nome": "Jonas Ferreira",
    "idade": 31,
    "perfil_renda": "PJ_MEI",
    "cidade": "Belo Horizonte-MG",
    "letramento_financeiro": "baixo_medio",
    "letramento_digital": "medio_alto",
    "canal": "whatsapp",
    "renda": [
      { "descricao": "servico_instalacao", "valor": 600.00, "data": "2026-10-22", "certeza": "certa" },
      { "descricao": "servico_manutencao", "valor": 350.00, "data": "2026-10-28", "certeza": "provavel" }
    ],
    "faturamento_6_meses": [2300, 1900, 1600, 1800, 2700, 3400],
    "data_decisao": "2026-10-15",
    "horizonte_ate": "2026-11-05",
    "saldo_conta": 2200.00,
    "fatura": { "valor": 2760.00, "minimo": 414.00, "vencimento": "2026-10-18", "limite": 4500.00 },
    "essenciais_ate_proxima_renda": [
      { "descricao": "aluguel", "valor": 750.00 },
      { "descricao": "pensao_alimenticia", "valor": 400.00 },
      { "descricao": "mercado", "valor": 330.00 },
      { "descricao": "combustivel_material", "valor": 250.00 },
      { "descricao": "luz", "valor": 90.00 },
      { "descricao": "das_mei", "valor": 86.00 },
      { "descricao": "internet", "valor": 60.00 }
    ],
    "reserva_minima": 150.00,
    "historico_2025": { "total": 5, "parcial": 4, "minimo": 3 },
    "evento_demo": { "descricao": "troca_pneu", "valor": 220.00 }
  }
]
```

**Parâmetros ilustrativos:** `juros_rotativo_am = 0.12`, `juros_parcelamento_am = 0.08`, `percentual_minimo = 0.15`.
