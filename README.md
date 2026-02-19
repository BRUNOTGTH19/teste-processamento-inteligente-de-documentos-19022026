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

# Teste — Extração de Dados de Fatura CEMIG

## Descrição do Projeto

Este projeto tem como objetivo desenvolver uma rotina em Python capaz de realizar a leitura da fatura `fatura_cemig.pdf` em formato PDF e extrair informações estruturadas relevantes.

O script utiliza a biblioteca `pdfplumber` para extração de texto e expressões regulares (`re`) para identificação e captura dos dados solicitados.

As informações extraídas são organizadas em um dicionário estruturado, exibidas no terminal e exportadas automaticamente para um arquivo `fatura_cemig.json`.

---

## Tecnologias Utilizadas

- Python 3
- pdfplumber
- re (expressões regulares)
- json
- decimal

---

## Informações Extraídas

O script extrai as seguintes informações da fatura:

1. Titular da fatura (Nome e Documento)
2. Endereço completo do titular
3. Classificação da Instalação
4. Número da instalação
5. Valor a pagar para a distribuidora
6. Data de vencimento
7. Mês ao qual a fatura é referente
8. Tarifa total com tributos
9. Tarifa total ANEEL
10. Quantidade em kWh do consumo da fatura
11. Saldo em kWh acumulado na instalação
12. Somatório das quantidades das energias compensadas (injetadas)
13. Somatório dos valores totais das operações (R$)
14. Contribuição de iluminação pública (CIP)
15. Alíquotas de ICMS, PIS e COFINS (%)
16. Linha digitável para pagamento

---

## Como Executar o Projeto

### 1️⃣ Pré-requisitos

- Python 3.10 ou superior instalado
- pip configurado no sistema

### 2️⃣ Instalação das Dependências

No terminal, execute:

```bash
{
    "Titular da Fatura": {
        "Nome": "JOAO NEVES",
        "Documento": "715.665.976-13"
    },
    "Endereço Completo": "PCA DOUTOR GONCALVES 379 CS 802 JUL/2023 06/08/2023 76,66 CENTRO 35570-000 VIÇOSA, MG",
    "Classificação da Instalação": "Residencial Residencial Convencional B1",
    "Número da Instalação": "12345678911",
    "Valor a Pagar para a Distribuidora (R$)": 76.66,
    "Data de Vencimento": null,
    "Mês de Referência": "JUL/2023",
    "Consumo da Fatura (kWh)": 199,
    "Saldo em kWh Acumulado na Instalação": 234.63,
    "Somatório Energias Compensadas (kWh)": 149,
    "Somatório Valores Totais das Operações (R$)": 623.85,
    "Contribuição de Iluminação Pública (R$)": 24.71,
    "Alíquotas (%)": {
        "ICMS": 0.0,
        "PIS": null,
        "COFINS": null
    },
    "Linha Digitável para Pagamento": "API22211117648"
}
pip install pdfplumber


# Teste 2

Contexto: Você recebeu a fatura "fatura_cemig.pdf" e deve desenvolver um script para extrair seus dados. Antes de iniciar a programação, é essencial compreender e interpretar as informações presentes nesta fatura.

Atividade: Analise a fatura e redija um documento respondendo os pontos abaixo. As respostas podem ser inseridas neste 'README'.

 - Identifique as principais diferenças entre a fatura "fatura_cemig.pdf" e uma fatura convencional de energia elétrica "fatura_cemig_convencional.pdf".
 - Descreva e explique os termos e valores apresentados na seção "Valores Faturados" da fatura "fatura_cemig.pdf".
 - Considerando que a instalação da "fatura_cemig.pdf" participa do Sistema de Compensação de Energia Elétrica, identifique e explique qual informação na seção "Informações Gerais" da fatura é considerada a mais importante.
 - Identifique o consumo da instalação referente ao mês de julho de 2023.

# Resposta para o Teste 2
Escreva aqui suas respostas para o teste 2.

# Requisitos dos Desafios:

1. Utilize a linguagem Python para desenvolver a solução.
2. No mesmo README, inclua uma seção detalhada que explique claramente os passos necessários para executar o código. Certifique-se de que as instruções sejam precisas, organizadas e fáceis de entender, pois os avaliadores seguirão essa documentação.
3. Faça um fork do repositório, para iniciar o desenvolvimento.
4. A entrega deve ser realizada por meio de um pull request para o repositório original. Caso não consiga, os arquivos podem ser enviados para o email falecom@dg.energy, porém com penalidade de pontos.
5. Abra o pull request também faltando 5 minutos para o prazo final da entrega do teste. Se o pull request for realizado antes dos 5 minutos restantes haverá eliminação do candidato.
6. A entrega deve ser realizada até às 12:30h.
