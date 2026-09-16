# Configuração de Memória do SanESocial

> 🔗 **Fonte:** [https://ajuda.sankhya.com.br/hc/pt-br/articles/38966117032087-Configura%C3%A7%C3%A3o-de-Mem%C3%B3ria-do-SanESocial](https://ajuda.sankhya.com.br/hc/pt-br/articles/38966117032087-Configura%C3%A7%C3%A3o-de-Mem%C3%B3ria-do-SanESocial)

---

# Configuração de Memória do SanESocial

#### **Windows** 

*   ##### Para configurar a memória do **SanESocial** no ambiente **Windows**, caso ele seja iniciado como serviço:
    

Exemplo: **\-J-Xms3072m -J-Xmx3072m**

![image - 2026-03-11T145752.128.png](https://ajuda.sankhya.com.br/hc/article_attachments/38967907057687)

*   Também é possível criar um arquivo com as configurações padrão. Na mesma pasta onde se encontra o launcher da aplicação, deve ser criado o arquivo **"sanesocial-service.vmoptions"**, contendo as configurações **Xms** e **Xmx**.
    

![image - 2026-03-11T145934.481.png](https://ajuda.sankhya.com.br/hc/article_attachments/38967931096343)

#### **Linux** 

*   No Linux basta alterar as propriedades **\-XMX** e -**XMS** do **sanesocial-service**.

![image - 2026-03-11T150138.801.png](https://ajuda.sankhya.com.br/hc/article_attachments/38967931100823)