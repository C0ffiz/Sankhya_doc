# Replay

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/15030110652439-Replay](https://ajuda.sankhya.com.br/hc/pt-br/articles/15030110652439-Replay)

---

# Replay

![Módulo 36x36 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/42310451077399) **Módulo:** Configurações > Avançado      ![Versão - 32x32 FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/42310511896855) **Versão disponível:** A partir da 4.20

---

![essencial FINAL (1).png](https://ajuda.sankhya.com.br/hc/article_attachments/16746821220759) É necessário habilitar o parâmetro **"Usa Sankhya Replay? - USASKREPLAY"** para que a referida tela funcione corretamente.

O objetivo da tela Replay será permitir a exportação de dados, registros e definições de parâmetros e objetos de banco, tais como: campos adicionais, triggers e procedures personalizados, e ainda, eventos Java não nativos de uma determinada base de dados e possibilitar a importação dos dados extraídos para outra base dados. 

**Nota:** é de suma importância que o usuário tenha conhecimento sobre a estrutura de dados para relacionar corretamente tabelas e colunas.

Dessa forma, na tela é possível executar processos com especificidades de informações a partir do “de-para” de dados de uma base para outra. Além disso, pode-se ainda, criar mapas de exportação para formar um conjunto de tabelas com ligações entre si a partir de uma tabela de origem. 

Sendo assim, teremos:

<table style="width: 100%; height: 44px;"><colgroup><col> <col> <col></colgroup><tbody><tr style="height: 22px;"><td style="width: 38.5714%; height: 22px;"><p><a href="#Exportar" target="_self" rel="undefined">Exportar</a></p></td><td style="width: 2.57143%; height: 22px;">&nbsp;</td><td style="width: 58.5714%; height: 22px;"><a href="#DesfazerImporta%C3%A7%C3%A3o" target="_self"><span style="background-color: #ffffff;">Desfazer Importação</span><strong><span style="background-color: #ffffff;">&nbsp;</span></strong></a></td></tr><tr style="height: 22px;"><td style="width: 38.5714%; height: 22px;"><a href="#Importar" target="_self"><span style="background-color: #ffffff;">Importar</span><strong><span style="background-color: #ffffff;">&nbsp;</span></strong></a></td><td style="width: 2.57143%; height: 22px;">&nbsp;</td><td style="width: 58.5714%; height: 22px;"><a href="#RegistrosExportados/Importados" target="_self"><span style="background-color: #ffffff;">Registros Exportados/Importados</span></a></td></tr></tbody></table>

## Exportar

O bloco **"Exportar"** permite a exportação de registros, objetos de banco e códigos Java personalizados.

![Exportar.png](https://ajuda.sankhya.com.br/hc/article_attachments/15029806554263)

No campo **"Mapa"**, informa-se um conjunto de tabela, das quais serão extraídos os dados de uma base de dados originária.  

Após definir o campo acima, será liberado o preenchimento do campo **"Tabela"**, nele é preciso escolher uma tabela base, sendo esta a referência para selecionar registros de outras tabelas com as quais possui vínculo.

No campo **"Condição"**, insira as cláusulas WHERE a fim de ampliar os critérios de seleção de dados.

Depois de preencher os campos acima, selecione as seguintes marcações conforme necessidade:

*   **Exportar Registro Padrão?:** por meio desta, o sistema permite a exportação de registros, a partir da tabela base, definida no campo Tabela;
*   **Exportar Campos Adicionais?:** esta marcação é usada para extrair os campos adicionais da base de dados de origem;
*   **Exportar Parâmetros?:** essa marcação possibilita a extração dos valores configurados nos parâmetros da base de dados originária;
*   **Exportar Eventos Personalizados?:** utiliza-se essa marcação para exportar procedures de banco de dados e código Java personalizados;
*   **Exportar Triggers Personalizadas?:** marcação usada para promover a exportação de Triggers não nativas da base de dados de origem.

[\[Voltar ao topo\]](#top)

## Importar

O bloco de **"Importação"** permitirá a importação de registros, objetos de banco e código JAVA personalizados.

![Importar.png](https://ajuda.sankhya.com.br/hc/article_attachments/15029818373527)

O campo **"Mapa"** é utilizado para definir o conjunto de tabela, das quais serão extraídos os dados de uma base de dados originária.

Já o campo **"Arquivo Originário"**, adicione o arquivo gerado na exportação dos dados feita anteriormente.

[\[Voltar ao topo\]](#top)

## Desfazer Importação

No bloco **"Desfazer Importação"**, pode-se desfazer as configurações dos valores dos parâmetros e remover objetos de banco de dados (Triggers e Procedures), criados a partir da importação supracitada.

![Desfazer\_importa\_\_o.png](https://ajuda.sankhya.com.br/hc/article_attachments/15029857586455)

No campo **"Arquivo Backup"** informa–se o arquivo de backup para restaurar os valores dos parâmetros, excluir triggers, procedures e eventos Java personalizados, sendo eles criados no ato da importação dos dados. 

[\[Voltar ao topo\]](#top)

## Registros Exportados/Importados

Para finalizar o preenchimento da tela, tem-se o bloco de **"Registros Exportados/Importados"**, ele possibilita a visualização dos registros e operação realizada na tela. 

![Registros\_Exportados\_Importados.png](https://ajuda.sankhya.com.br/hc/article_attachments/15029879222679)

Na coluna **"Tipo de processo"** a etapa de exportação é, objetivamente, definida com o mesmo nome enquanto a etapa de importação é nomeada como **"Importação"** sugestivamente.

[\[Voltar ao topo\]](#top)

![acesse também FINAL.png](https://ajuda.sankhya.com.br/hc/article_attachments/16746803029783) Confira também: 

[Mapa de Exportação Replay](https://ajuda.sankhya.com.br/hc/pt-br/articles/15031231465751-Mapa-de-Exporta%C3%A7%C3%A3o-Replay)