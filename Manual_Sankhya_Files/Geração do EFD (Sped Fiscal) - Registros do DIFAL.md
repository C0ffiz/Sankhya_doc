# Geração do EFD (Sped Fiscal) - Registros do DIFAL

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/360044600654-Gera%C3%A7%C3%A3o-do-EFD-Sped-Fiscal-Registros-do-DIFAL](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044600654-Gera%C3%A7%C3%A3o-do-EFD-Sped-Fiscal-Registros-do-DIFAL)

---

# Geração do EFD (Sped Fiscal) - Registros do DIFAL

Foi publicado (na data de 06/01/2016) o novo Guia da EFD contendo as detalhamento das especificações técnicas publicadas no Ato Cotepe ICMS nº 61, de 30 de dezembro de 2015 (DOU 31/12/2015) que tem por objetivo atender as alterações da Emenda Constitucional nº 87/2015.

A Emenda Constitucional nº 87 contempla as alterações de ICMS para operações interestaduais destinadas ao consumidor final não contribuinte do imposto. Ela trata da sistemática de cobrança do imposto sobre operações relativas à circulação de mercadorias e sobre prestações de serviços de transporte interestadual e intermunicipal e de comunicação incidente sobre as operações e prestações que destinem bens e serviços a consumidor final, não do imposto, localizado em outro Estado.

Visando atender esta emenda, foram incluídos os seguintes registros:

*   C101;
*   D101;
*   E300;
*   E310;
*   E311;
*   E312;
*   E313;
*   E316.

Além disso, para o "Bloco K", tem-se a obrigatoriedade de "Abertura" e "Fechamento" dos registros.

As informações aqui apresentadas, estão relacionadas à "[Nota Técnica 2015.003 - NF-e, CEST e DIFAL Partilhado](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044600414-Nota-T%C3%A9cnica-2015-003-NF-e-CEST-e-DIFAL-Partilhado)".

Atenção Consultor Sankhya: O sistema conta com a Apuração para o DIFAL; para geração dos dados, deve-se seguir o processo já existente. Contudo, a apuração do ICMS é feita de forma geral, ou seja, a UF não é considerada (a apuração é salva na TGFAJA com CODUF = 0 e TIPIMPOSTO = 'C' - ICMS), conforme exemplo abaixo:

![img01.png](https://ajuda.sankhya.com.br/hc/article_attachments/8983240370967)

Para o DIFAL, esses dados são salvos por UF; vejamos abaixo um exemplo dos registros salvos para o TIPIMPOSTO = 'D' (ICMS DIFAL) e para UF's distintas - "1 (SP)" e "2 (MG)":

![img02.png](https://ajuda.sankhya.com.br/hc/article_attachments/8983483273623)

Do mesmo modo é feito para o TIPIMPOSTO = 'F' (ICMS FCP). No exemplo abaixo, não houve cálculo do Fundo de Combate à Pobreza para UF = 1 (SP), somente para UF = 2 (MG):

![img03.png](https://ajuda.sankhya.com.br/hc/article_attachments/8983537638295)

Os dados apresentados acima, foram gerados por meio do seguinte processo:

•Efetua-se o lançamento de notas para determinada empresa (Tela - Portais);

•Faz-se a geração do Livro Fiscal para a empresa, gravando-se assim, os dados na TGFLIV (Tela "[Livros Fiscais > Arquivos > Geração ICMS/IPI](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045115953-Gera%C3%A7%C3%A3o-ICMS-IPI)");

•Feita a apuração do ICMS para empresa em determinado período, grava-se os dados na tabela TGFAJA (Tela "[Livros Fiscais > Relatórios > Registro de Apuração do ICMS](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045116153-Registro-de-Apura%C3%A7%C3%A3o-do-ICMS)").

A apuração realizada pela tela "Registro de Apuração do ICMS" não gera dados para todos os tipos de apuração. Para o ICMS são gravados na tabela TGFAJA os seguintes Tipos de Apuração:

1 - Saídas com Débito do Imposto;

4 - Total Débitos;

5 - Entradas com Crédito do Imposto;

8 - Sub Total;

9 - Saldo Credor do Período Anterior;

10 - Total Créditos;

11 - SALDO DEVEDOR (Débito - Crédito);

13 - IMPOSTO A RECOLHER;

14 - SALDO CREDOR (Crédito - Débito) a Transportar;

15 - Saldo Credor Produzir do Período Anterior.

Para o ICMS DIFAL e ICMS FCP são gravados os mesmos tipos de apuração apresentados acima, com exceção do Tipo de Apuração "15 -  Saldo Credor Produzir do Período Anterior".

Os outros tipos de apuração podem ser inseridos através da tela "Livros Fiscais > Arquivos > Ajuste da Apuração de ICMS e ICMS ST". São eles:

2 - Outros débitos;

3 - Estorno de créditos;

6 - Outros créditos;

7 - Estorno de débitos;

12 - Deduções do imposto apurado;

100 - Débito especial;

101 - Controle do ICMS extra-apuração.