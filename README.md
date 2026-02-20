# Returning-an-XML-in-the-Message-Body
SAP BTP CPI - Retornando um XML no Corpo da Mensagem


![Capa](imagens/capa-linkedin.png)


📊 Exemplo Prático do Fluxo

### Criando nosso Iflow
![Fluxo](imagens/Screenshot_1.png)

### Adicionando o nome para iFlow
![Fluxo](imagens/Screenshot_2.png)

### Editando nosso Iflow
![Fluxo](imagens/Screenshot_3.png)

### Adicionando o Content Modifier
![Fluxo](imagens/Screenshot_4.png)

### Renomeando nosso Content Modifier
![Fluxo](imagens/Screenshot_5.png)

### Adicionando no corpo nossa mensagem no Content Modifier
Vamos em Message Body, que será o corpo do Messagem em XML
``` 
<root>
   <message>${body}</message>
</root>

```
![Fluxo](imagens/Screenshot_6.png)

### Retornando o xml no nosso Iflow
Message Header - Content-Type - Constant - application/xml
![Fluxo](imagens/Screenshot_7.png)

### Salvar e Deploy
![Fluxo](imagens/Screenshot_8.png)

### Salvando e Deploy as configurações realizadas
![Fluxo](imagens/Screenshot_9.png)

### Conectando Sender no Start
![Fluxo](imagens/Screenshot_10.png)

### Selecionar o HTTPS
![Fluxo](imagens/Screenshot_11.png)

### Adicionando o Endereço para no Iflow
Salvar e Deploy
![Fluxo](imagens/Screenshot_12.png)

### Deployment Status
Para adicionar nosso XML
![Fluxo](imagens/Screenshot_13.png)

### Endpoint
![Fluxo](imagens/Screenshot_14.png)

### Configuração no Postman
Adicionar a URL do Endpoint
![Fluxo](imagens/Screenshot_15.png)





## 📦 Exemplo prático – iFlow para baixar

📦 [Download do iFlow – Package/FilterwithXML.zip](Package/FilterwithXML.zip)



> O arquivo pode ser importado diretamente no SAP Integration Suite (CPI).
