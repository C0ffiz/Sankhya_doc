# Geração ISS

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/360044607514-Gera%C3%A7%C3%A3o-ISS](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044607514-Gera%C3%A7%C3%A3o-ISS)

---

# Geração ISS

![Módulo 36x36 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/42312940023191) **Módulo:** Livros Fiscais > Arquivos

---

Por meio desta tela, você pode realizar a geração das notas fiscais de serviço no módulo dos livros fiscais. Seu objetivo é que as notas fiscais que possuem serviços, confirmadas e/ou autorizadas (no caso de NFS-e - Notas Fiscais de Serviço Eletrônica), sejam geradas (alimentando a tabela TGFLIS), ficando deste modo disponíveis para as demais funcionalidades do sistema, **"Relatório Livro ISS"** (em construção) e **"EFD Contribuições"** (bloco A).

![iss.png](https://ajuda.sankhya.com.br/hc/article_attachments/7887822729111)

Inicialmente, informe a **"Empresa"** bem como a **"Empresa Destinatária"**, ou seja, a empresa pela qual realizou a emissão das notas.

Determine em seguida, o período que o sistema irá filtrar as notas para geração das informações. Esse dado é fornecido por meio dos campos **"Data Inicial"** e **"Data Final"**.

Tem-se a possibilidade de geração de uma única nota, ao informar seu **"Número Único"**, onde o sistema irá buscar apenas o documento correspondente a numeração indicada. 

**Seção Ações**

Nesta seção, determine os conjuntos de dados relacionados às notas que serão gerados. Pode-se definir dentre as seguintes marcações:

*   **Gerar Notas:** serão geradas todas as informações referentes às notas, dentro do período estabelecido.
*   **Gerar Canceladas:** com esta marcação, serão consideradas apenas as notas canceladas dentro do período definido.
*   **Gerar Financeiro:** será considerado para geração, apenas o financeiro das notas contidas no período estabelecido.
*   **Gerar Redução Z:** serão gerados os fechamentos fiscais diários de um ECF (Emissor de Cupom Fiscal), visto que este trabalha com base em movimentações diárias.

**Seção Filtros**

Neste trecho, determine qual operação será considerada para geração dos dados. Pode-se marcar uma ou ambas as opções, que são:

*   **Aquisições:** Serão considerados apenas os serviços adquiridos (entrada);
*   **Prestações:** É feita a busca pelos serviços fornecidos (saída).

Sobre a Geração de ISS têm-se os seguintes pontos:

*   Inicialmente, o sistema buscará as notas que possuam pelo menos um item de serviço e estão conforme as regras para serem geradas no livro.
*   Logo após, se a marcação **"Gerar notas com ISS zerado"** estiver habilitada o sistema buscará as notas que possuem a configuração para serem geradas no livro, ainda que estas não tenham item de serviço. Sendo assim, as notas que ainda não foram geradas, irão para o livro com apenas um item e os campos **"Base"**, **"Alíquota"** e **"Valor ISS"** zerados.

**Botões da tela**

Uma vez definidas as configurações até aqui mencionadas, por meio do botão ![gerar-agora-FINAL.jpg](https://ajuda.sankhya.com.br/hc/article_attachments/16313610651287) **"Gerar Agora"**, efetue a geração das informações pertinentes às notas de serviço.

Quando o botão ![consultar-nota-não-gerada-FINAL.jpg](https://ajuda.sankhya.com.br/hc/article_attachments/16313686338071)  **"Consultar Nota Não Gerada"** for acionado, permite a consulta de alguma nota que não tenha sido gerada no livro de ISS. Será aberto um pop-up também de nomenclatura Consultar Nota Não Gerada, onde pode-se utilizar dos seguintes dados para buscar as notas:

*   Nro. único;
*   Chave NFe\\CTe;
*   Nro. Nota;
*   Série;
*   Data de Negociação;
*   Empresa.

Os três últimos campos de filtragem serão habilitados para preenchimento, apenas se o Nro. Nota for primeiramente informado.

Acionando o botão ![botao-agendamento-FINAL.jpg](https://ajuda.sankhya.com.br/hc/article_attachments/16313808835223) **"Agendamento"**, você será direcionado para a tela [Geração ISS Agendamento](https://ajuda.sankhya.com.br/hc/pt-br/articles/7869194336407-Gera%C3%A7%C3%A3o-ISS-Agendamento). 

[\[Voltar ao topo\]](#top)