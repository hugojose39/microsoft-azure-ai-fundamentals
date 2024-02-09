<h1>
    <a href="https://www.dio.me/">
     <img align="center" width="60px" src="https://hermes.dio.me/lab_projects/badges/619af8f8-d138-4e40-9d48-fec7b318e44d.png"></a>
    <span> 
Azure Cognitive Search: Utilizando AI Search para indexação e consulta de Dados</span>
</h1>

## Problema:

O desafio propõe a criação de uma pesquisa que opere em conjunto com um serviço de inteligência artificial para identificar palavras-chave, analisar sentimentos e aproveitar o serviço de armazenamento do Azure.

[Documentação](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/11-ai-search.html)

## Passo 1: Criando recurso do Azure AI Search:

<img src="./images/1.png"/>
<img src="./images/2.png"/>
<img src="./images/3.png"/>
<img src="./images/4.png"/>
<img src="./images/5.png"/>
<img src="./images6/.png"/>

## Passo 2: Criando recurso do Azure AI services:

<img src="./images/7.png"/>
<img src="./images/8.png"/>
<img src="./images/9.png"/>

## Passo 3: Criando o storage:

<img src="./images/10.png"/>
<img src="./images/11.png"/>
<img src="./images/12.png"/>
<img src="./images/13.png"/>

## Passo 4: Permitindo acesso anônimo ao Blob:

Dado que nosso laboratório é estritamente educacional, com o intuito de compreender os fundamentos da inteligência artificial com o Azure, é necessário habilitar o acesso anônimo ao blob para simplificar e agilizar nossas implementações. Após criar o seu armazenamento, acesse o mesmo e siga até a guia SETTINGS > CONFIGURATION conforme os passos abaixo:Dado que nosso laboratório é estritamente educacional, com o intuito de compreender os fundamentos da inteligência artificial com o Azure, é necessário habilitar o acesso anônimo ao blob para simplificar e agilizar nossas implementações. Após criar o seu armazenamento, acesse o mesmo e siga até a guia SETTINGS > CONFIGURATION conforme os passos abaixo:

<img src="./images/14.png"/>
<img src="./images/15.png"/>

## Passo 5: Criando o Container:

Dirija-se à aba DATA STORAGE > CONTAINERS para estabelecer o contêiner dentro do armazenamento e incluir as pesquisas que serão analisadas pelo serviço de IA.

<img src="./images/16.png"/>
<img src="./images/17.png"/>
<img src="./images/18.png"/>
<img src="./images/19.png"/>
<img src="./images/20.png"/>

## Passo 6: Importação e indexação dados para o AI SEARCH:      

Neste estágio, é necessário vincular / importar os dados que foram inseridos e configurados no seu armazenamento. Em seguida, retorne para o AI SEARCH e prossiga com os passos a seguir:

<img src="./images/21.png"/>
<img src="./images/22.png"/>
<img src="./images/23.png"/>

Esta etapa é crucial em todo o processo, como destacado no bootcamp. São muitos passos que precisam ser seguidos meticulosamente. É importante observar que podem haver algumas diferenças entre a documentação oficial e o que você encontrou ao configurar o seu sistema.

Ao seguir a [Documentação](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/11-ai-search.html) você chegará em INDEX DOCUMETS, o qual o gif acima mostra o início do processo, siga os topicos até chegar na sessão 4:

<img src="./images/24.png"/>

**4. In the Attach Cognitive Services section, select your Azure AI services resource.**

Observe que as instruções pedem que você selecione o recurso AI SERVICE configurado. No entanto, pode ser que você não veja nenhum recurso disponível, apenas uma informação indicando que o acesso é gratuito e as configurações são limitadas. Não se preocupe com isso e prossiga para o Passo 5 . In the Add enrichments section.

Continue seguindo todas as configurações conforme indicado, concluindo no Passo 17. Select the indexer name to see more details.

## Passo 7: Consultando o índice:      

Após realizar todas as configurações, retorne ao AZURE AI SERVICES e acesse o nosso serviço. Utilize o SEARCH EXPLORER para testar se todos os dados foram indexados corretamente e se as consultas estão funcionando conforme o esperado, utilizando os comandos adequados.

<img src="./images/25.png"/>

```
search=*&$count=true    (  verifica se a indexação esta funcionando e mostra os documentos )
```
<img src="./images/26.png"/>

```
search=locations:'Chicago' ( Consulta as ocorrências acontecidas em Chicado )
```
<img src="./images/27.png"/>

## Observações finais:      

As ferramentas de inteligência artificial do Azure simplificam a consulta em documentos, pesquisas e depoimentos, tornando mais eficiente a análise da satisfação das empresas em relação aos seus produtos e serviços.


