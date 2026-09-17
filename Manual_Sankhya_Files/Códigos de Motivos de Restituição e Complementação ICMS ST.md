# Códigos de Motivos de Restituição e Complementação ICMS ST

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/4414035288727-C%C3%B3digos-de-Motivos-de-Restitui%C3%A7%C3%A3o-e-Complementa%C3%A7%C3%A3o-ICMS-ST](https://ajuda.sankhya.com.br/hc/pt-br/articles/4414035288727-C%C3%B3digos-de-Motivos-de-Restitui%C3%A7%C3%A3o-e-Complementa%C3%A7%C3%A3o-ICMS-ST)

---

# Códigos de Motivos de Restituição e Complementação ICMS ST

<table style="border-collapse: collapse; width: 99.9977%;"><tbody><tr><td style="width: 99.8571%;"><pre><span class="wysiwyg-font-size-medium"><strong><img src="https://ajuda.sankhya.com.br/hc/article_attachments/16282679000471" alt="Módulo 36x36 FINAL.png"> Módulo: </strong>Livros Fiscais &gt; Avançado &gt; Escrituração Fiscal Digital  <strong><br><img src="https://ajuda.sankhya.com.br/hc/article_attachments/16282679002263" alt="Versão - 32x32 FINAL.png"> Versão disponível: </strong>a partir da 4.7</span></pre></td></tr></tbody></table>

---

Nesta tela você poderá cadastrar todos os Códigos de Motivos de Restituição e Complementação de ICMS ST. Assim, ao acessar a tela inicial da rotina, a pesquisa poderá ser efetuada usando o próprio código ou a **"Sequência"** de numeração cadastrada.

Para inserir um código novo, clique no botão **"Adicionar"** e preencha os campos abaixo:

![mceclip10.png](https://ajuda.sankhya.com.br/hc/article_attachments/4414031938199)  
Você poderá configurar a Sequência de numeração dos registros para ser gerada automaticamente pelo sistema ou para que seja informada manualmente, por meio do botão ![botão-configuração-da-tela-FINAL.jpg](https://ajuda.sankhya.com.br/hc/article_attachments/16284152665879) **"Configuração da tela"**, localizado na barra de ferramentas desta tela.

Nos campos **"Data de Início"**, **"Data de Fim"**, **"Código do Ajuste"** e **"Descrição do Ajuste"**, preencha as informações do código que deseja cadastrar, conforme descrito na Tabela 5.7 do EFD ICMS/IPI.

Selecione a **"Empresa"** para qual deseja cadastrar o código.

Escolha o **"CFOP"** para utilizar o código cadastrado numa determinada CFOP.

Indique o **"Cód.Tipo Operação"**. Caso este campo não seja preenchido, não haverá restrição por TOP.

Selecione a **"Classificação do ICMS"** de acordo com as seguintes opções:

*   Isento de ICMS;
*   Consumidor Final Não Contribuinte;
*   Revendedor;
*   Consumidor Final Contribuinte;
*   Produtor Rural;
*   Sem classificação.

Informe a **"Finalidade da Operação"**, para que seja apresentada no cabeçalho da nota.

Preencha no campo **"UF de origem"**, o estado a que pertence o código do motivo de restituição que está sendo cadastrado.

Você poderá adicionar um **"Filtro personalizado"** a fim de atender as regras de negócio do código configurado.

---

#### **Requisitos da rotina**

Para que o sistema utilize o código cadastrado, atente-se aos requisitos abaixo:

*   Na geração do EFD Fiscal, o sistema verifica se o período de geração do arquivo está entre as Data de Início e Data de Fim do código cadastrado. Caso contrário, o código não poderá ser utilizado.
*   Se o campo Empresa estiver preenchido, utilizará o código do ajuste cadastrado para ela. Ficando em branco, este código será utilizado para todas as empresas do estado.
*   Com o campo CFOP preenchido, o sistema só poderá usar o código do ajuste cadastrado para ele, caso não preencha, não haverá restrição por CFOP.
*   Se o campo Classificação do ICMS estiver preenchido, o sistema irá validar se a classificação de ICMS do Parceiro da nota é a mesma. Essa validação poderá ocorrer em três cadastros diferentes:

1.   Primeiramente, no cadastro da TOP, aba [Impostos](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044603114-Tipos-de-Opera%C3%A7%C3%A3o-TOP#abaimpostos), no campo **"Classificação ICMS"** deverá estar selecionada a opção **"Usar do Parceiro"**, do contrário, a nota não aceitará essa restrição.

2.  Depois, se no cadastro da TOP, o campo Classificação ICMS estiver com a opção Usar do Parceiro, então o sistema verificará se no cadastro do Parceiro, aba [Grupo ICMS/ISS por Empresa](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044594494-Cadastro-de-Parceiros#abagrupoicmsissporempresa) tem a mesma classificação, assim utilizará o código configurado.

3.   Caso no cadastro da TOP, o campo Classificação ICMS esteja em branco, o sistema verificará no cadastro do Parceiro, aba [Fiscal](https://ajuda.sankhya.com.br/hc/pt-br/articles/360044594494-Cadastro-de-Parceiros#abafiscal) se é a mesma Classificação ICMS cadastrado nesta rotina.

*   Se a Finalidade da Operação estiver selecionada, o sistema validará se o campo de mesma nomenclatura no cabeçalho da nota está preenchido com a mesma opção para usar essa restrição, caso contrário, não será utilizada.

---

#### **Botões da tela**

O botão ![botao-exibe-os-registros-marcados-como-favoritos-FINAL.jpg](https://ajuda.sankhya.com.br/hc/article_attachments/16282906298135) **"Exibe os registros marcados como favoritos"** anteriormente. Observe como realizar esta marcação através do link [Marcar um registro como Favorito](https://ajuda.sankhya.com.br/hc/pt-br/articles/360045110733-HTML5#marcarumregistrocomofavorito).

Ao clicar no botão ![botao-exibe-os-registros-recentemente-editados-FINAL.jpg](https://ajuda.sankhya.com.br/hc/article_attachments/16283514590871) **"Exibe os registros recentemente editados"**, serão apresentados os registros em que foram alteradas informações recentes.

Este botão, ![botao-exportar-grade-para-pdf-FINAL.jpg](/guide-media/01H6743AM7C5181E5VX745E5ZA) **"Exportar grade para PDF"** apresenta opções de exportação e visualização das informações da tela. Você poderá **"Exportar para PDF"**, **"Exportar para planilha"** ou **"Exportar para cubo"**.

Por meio do botão ![botao-anexo-FINAL.jpg](/guide-media/01H6748806TF4YTBWEJSKWJX68) **"Anexo"**, você poderá anexar algum documento relevante para esta rotina.

---

#### **Informações adicionais**

*   **Registro C185: Informações complementares das operações de saída de mercadorias.**  
    Se o terceiro caractere do campo **"Código do Ajuste"** for 0, 1, 2 ou 3, ele só poderá ser usado no registro C185 do Sped Fiscal, no registro de número 06.
*   **Registro C181: Informações complementares das operações de devoluções de saída de mercadorias.**  
    Se o terceiro caractere do campo Código do Ajuste for 5, 6, 7 ou 8, então só poderá ser usado no registro C181 do Sped Fiscal, no registro de número 02.
*   **Registro C186: Informações complementares das operações de devoluções de entrada de mercadorias.**  
    Se o terceiro caractere do campo Código do Ajuste for 4, só poderá ser usado no registro C186 do Sped Fiscal, no registro de número 02.

![essencial FINAL (1).png](https://ajuda.sankhya.com.br/hc/article_attachments/16283955868823) Os códigos de motivo influenciam no preenchimento de alguns campos em determinados registros, para verificar essa rotina consulte o [Guia Prático EFD Versão 3.1.4](https://drive.google.com/file/d/1cuvq0RTqjpZuMu8VW2Qbd2CkbWYZXmxX/view?usp=drive_link).

[\[Voltar ao topo\]](#top)