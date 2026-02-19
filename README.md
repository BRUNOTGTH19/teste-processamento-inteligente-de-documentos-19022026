# Teste Técnico (Extração de informações em Faturas de Energia)

Para garantir o eficiente gerenciamento dos créditos de energia provenientes de usinas de energia renovável, é fundamental a extração precisa e automática de dados das notas fiscais de energia elétrica. Além disso, possuir conhecimento sobre faturas de energia elétrica é importante para o sucesso na gestão desses recursos.

Logo, é proposto dois testes como parte da avaliação dos conhecimentos técnicos e teóricos dos candidatos. Essa avaliação tem o objetivo de medir a compreensão do participante no contexto da extração de dados de notas fiscais e no entendimento básico de faturas de energia elétrica.

# Teste 1

Em busca pela eficiência na leitura de faturas, a equipe de desenvolvimento propõe a criação de uma rotina que, a partir de faturas de energia elétrica em formato de PDF, seja capaz de extrair importantes informações.

Nesta atividade, você deve editar o arquivo read.py e desenvolver uma rotina capaz de realizar a leitura da fatura fatura_cpfl.pdf em formato de PDF e retornar as seguintes informações:

- Titular da fatura (Nome e Documento)
- Endereço completo do titular da fatura
- Classificação da Instalação
- Número da instalação
- Valor a Pagar para a distribuidora
- Data de Vencimento
- Mês ao qual a fatura é referente
- Tarifa total com tributos
- Tarifa total Aneel
- Quantidade em kWh do Consumo da fatura
- Saldo em kWh acumulado na Instalação
- Somatório das quantidades das energias compensadas (injetadas)
- Somatório dos Valores Totais das Operações R$
- Contribuição de iluminação Pública
- Alíquotas do ICMS, PIS e COFINS em %
- Linha digitável para pagamento

Organize a saída e visualização das informações extraídas.

# Documentação do Teste 1

Escreva aqui a documentação do desenvolvimento do teste 1.

# Teste 2

Contexto: Você recebeu a fatura "fatura_cemig.pdf" e deve desenvolver um script para extrair seus dados. Antes de iniciar a programação, é essencial compreender e interpretar as informações presentes nesta fatura.

Atividade: Analise a fatura e redija um documento respondendo os pontos abaixo. As respostas podem ser inseridas neste 'README'.

 - Identifique as principais diferenças entre a fatura "fatura_cemig.pdf" e uma fatura convencional de energia elétrica "fatura_cemig_convencional.pdf".
 - Descreva e explique os termos e valores apresentados na seção "Valores Faturados" da fatura "fatura_cemig.pdf".
 - Considerando que a instalação da "fatura_cemig.pdf" participa do Sistema de Compensação de Energia Elétrica, identifique e explique qual informação na seção "Informações Gerais" da fatura é considerada a mais importante.
 - Identifique o consumo da instalação referente ao mês de julho de 2023.

1. Diferenças entre a fatura fatura_cemig.pdf e uma fatura convencional de energia elétrica (fatura_cemig_convencional.pdf)

A fatura fatura_cemig.pdf refere-se a uma unidade consumidora participante do Sistema de Compensação de Energia Elétrica (SCEE), enquanto a fatura fatura_cemig_convencional.pdf corresponde a uma unidade consumidora convencional, sem geração própria de energia.

As principais diferenças observadas são:

A fatura com compensação apresenta lançamentos de energia injetada na rede, como Energia compensada GD II e Energia compensada adicional, inexistentes na fatura convencional;

Existe a indicação explícita de saldo de energia de geração (kWh) na fatura com compensação, o que não ocorre na fatura convencional;

O valor total a pagar na fatura com compensação é significativamente menor, pois parte do consumo é abatida por créditos de energia gerada;

A fatura convencional apresenta apenas a cobrança integral da energia consumida, sem créditos ou saldo acumulado;

A fatura com compensação possui maior complexidade no detalhamento dos valores faturados, refletindo a separação entre consumo, injeção de energia e compensações.

Essas diferenças evidenciam o impacto direto da geração distribuída no faturamento da energia elétrica.

2. Descrição e explicação da seção “Valores Faturados” da fatura fatura_cemig.pdf

A seção “Valores Faturados” da fatura fatura_cemig.pdf apresenta o detalhamento financeiro da energia consumida, compensada e dos encargos aplicáveis. Os principais itens são:

Energia Elétrica: refere-se à energia efetivamente consumida da rede da distribuidora.

Energia SCEE s/ ICMS: energia consumida no âmbito do Sistema de Compensação de Energia Elétrica, com tratamento tributário diferenciado.

Energia compensada GD II: energia injetada na rede pela unidade consumidora e utilizada para compensar o consumo faturado, apresentada com valor negativo.

Energia compensada adicional: complemento da compensação de energia, também abatendo o valor da fatura.

Bônus Itaipu (art. 21 da Lei 10.438): benefício concedido aos consumidores, reduzindo o valor total da fatura.

Contribuição de Iluminação Pública (CIP): taxa municipal destinada ao custeio da iluminação pública.

TOTAL: valor final da fatura após a aplicação de todas as compensações, bônus e encargos.

Essa seção demonstra claramente como a energia gerada e injetada na rede reduz o valor final a ser pago pelo consumidor.

3. Informação mais importante na seção “Informações Gerais” considerando o Sistema de Compensação de Energia Elétrica

Na fatura fatura_cemig.pdf, a informação mais relevante na seção “Informações Gerais” é o Saldo Atual de Geração, expresso em kWh.

Esse saldo indica a quantidade de energia excedente gerada pela unidade consumidora que permanece disponível para compensar consumos futuros. Ele é considerado o dado mais importante porque:

Determina o potencial de abatimento nas próximas faturas;

Representa o benefício econômico direto da geração distribuída;

Está sujeito a regras de validade e expiração;

Influencia diretamente o planejamento de consumo do consumidor.

Sem esse saldo, não seria possível avaliar a eficiência do sistema de compensação nem prever o impacto financeiro futuro.

4. Consumo da instalação no mês de julho de 2023

Com base no Histórico de Consumo apresentado na fatura fatura_cemig.pdf, o consumo da instalação referente ao mês de julho de 2023 foi de:

199 kWh

Esse valor corresponde à energia consumida no período, antes da aplicação das compensações provenientes da energia gerada e injetada na rede .

Considerações Finais

A análise das faturas evidencia as diferenças estruturais e financeiras entre uma unidade consumidora convencional e uma unidade participante do Sistema de Compensação de Energia Elétrica, destacando os benefícios econômicos da geração distribuída e a importância do controle do saldo de energia acumulado.


# Requisitos dos Desafios:

1. Utilize a linguagem Python para desenvolver a solução.
2. No mesmo README, inclua uma seção detalhada que explique claramente os passos necessários para executar o código. Certifique-se de que as instruções sejam precisas, organizadas e fáceis de entender, pois os avaliadores seguirão essa documentação.
3. Faça um fork do repositório, para iniciar o desenvolvimento.
4. A entrega deve ser realizada por meio de um pull request para o repositório original. Caso não consiga, os arquivos podem ser enviados para o email falecom@dg.energy, porém com penalidade de pontos.
5. Abra o pull request também faltando 5 minutos para o prazo final da entrega do teste. Se o pull request for realizado antes dos 5 minutos restantes haverá eliminação do candidato.
6. A entrega deve ser realizada até às 12:30h.
