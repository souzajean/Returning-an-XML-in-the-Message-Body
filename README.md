# Returning-an-XML-in-the-Message-Body
SAP BTP CPI - Retornando um XML no Corpo da Mensagem

Returning an XML Payload do Postman in the Message Body 



![Capa](imagens/capa-linkedin.png)


📊 Exemplo Prático do Fluxo

### Criando nosso Iflow
![Fluxo](imagens/Screenshot_1.png)

### Adicionando o nome para nosso Pacote
![Fluxo](imagens/Screenshot_2.png)

### Criando nosso Artefato do iFlow
![Fluxo](imagens/Screenshot_3.png)

### Adicionando o Integration Flow
![Fluxo](imagens/Screenshot_4.png)

### Editando nosso Iflow
![Fluxo](imagens/Screenshot_5.png)

### Removendo o Sender do nosso iFlow
![Fluxo](imagens/Screenshot_6.png)

### Removendo o Receiver do nosso iFlow
![Fluxo](imagens/Screenshot_7.png)

### Adicionando o Filter ao nosso Iflow
![Fluxo](imagens/Screenshot_8.png)

### Renomeando o Filter para Filter XML
![Fluxo](imagens/Screenshot_9.png)

### Realizando o Filter 
Nesta etapa iremos colocar o caminho do XML que queremos filtrar

> Filter - Processing

```
XPath Expression: /empregados/empregado[estado = 'SP']
```
📌 Importante:
XPath não transforma XML, ele apenas seleciona nós.

![Fluxo](imagens/Screenshot_10.png)

### Arquivo do empregados.xml

``` empregados.xml
<?xml version='1.0' encoding='UTF-8'?>
<empregados>
</empregados>

```
![Fluxo](imagens/Screenshot_11.png)

### Selecionando Conector
![Fluxo](imagens/Screenshot_12.png)

### Clicar no icone de iniciar Simulação
Para adicionar nosso XML
![Fluxo](imagens/Screenshot_13.png)

### Adicionando o conteúdo do empregados.xml
![Fluxo](imagens/Screenshot_14.png)

### Clicar no Conector e adicionar o End Simulação
![Fluxo](imagens/Screenshot_15.png)

### Clicar para iniciar nossos teste de simulação
![Fluxo](imagens/Screenshot_16.png)

### Clicar no Envelope para ver o resultado
![Fluxo](imagens/Screenshot_17.png)

### Resultado com o filtro do XML
Com todos os dados que são do estado de SP
![Fluxo](imagens/Screenshot_18.png)

### XML do resultado
![Fluxo](imagens/Screenshot_19.png)

``` Resultado do Filtro de SP
<?xml version='1.0' encoding='UTF-8'?>
<empregados>
  </empregados>
```



## 📦 Exemplo prático – iFlow para baixar

📦 [Download do iFlow – Package/FilterwithXML.zip](Package/FilterwithXML.zip)



> O arquivo pode ser importado diretamente no SAP Integration Suite (CPI).
