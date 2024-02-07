<h1>
    <a href="https://www.dio.me/">
     <img align="center" width="60px" src="https://hermes.dio.me/lab_projects/badges/87d332d0-5198-4a2f-b159-38c8c2976954.png"></a>    <span> Trabalhando com Machine Learning</span>
</h1>

## Criando modelo de previsão - Passo a passo

Para trabalhar com machine learning, é essencial que você possua um workspace. Esta é a tarefa inicial: criar o seu workspace para poder automatizar seu trabalho.

Depois que nosso workspace estiver pronto, devemos entrar no ML studio para criar um "novo trabalho de ML automatizado", seguindo o passo a passo da documentação do Learning para melhor entendimento e para que tudo dê certo:

![Passo 1](./images/01.png)

### Vamos criar um aprendizado de máquina para a previsão de aluguel de bicicletas:

![Passo 2](./images/02.png)

O tipo de tarefa é regressão e o nome de ativo de dados é aluguel de bicicletas, com fonte de dados da web.

![Passo 3](./images/03.png)
![Passo 4](./images/04.png)
![Passo 5](./images/05.png)
![Passo 6](./images/06.png)

A documentação do Learning é bem didática e traz todos os valores e configurações para que o trabalho automatizado seja criado:

![Passo 7](./images/07.png)
![Passo 8](./images/08.png)
![Passo 9](./images/09.png)
![Passo 10](./images/10.png)
![Passo 11](./images/11.png)
![Passo 12](./images/12.png)
![Passo 13](./images/13.png)

Chegando na opção "examinar", basta enviar o seu trabalho de treinamento:

![Passo 14](./images/14.png)

Após enviar, seu trabalho irá passar pelo processo de configuração das execuções e, após 15, podendo o tempo ser menor, estará concluído:

![Passo 15](./images/15.png)
![Passo 16](./images/16.png)

Pipeline com as etapas do processo de aprendizado e os testes realizados

![Passo 17](./images/17.png)

## Teste do modelo

Na página do modelo, cliquei na aba "Pontos de extremidade". Também é possível acessar pelo menu lateral em "Pontos de extremidade". Cliquei no ponto correspondente ao modelo gerado. Em seguida, acessei a aba "Testar".

Para o teste, utilizei o json abaixo:

```json
{
  "input_data": {
    "data": [
       {
         "day": 1,
         "mnth": 1,   
         "year": 2022,
         "season": 2,
         "holiday": 0,
         "weekday": 1,
         "workingday": 1,
         "weathersit": 2, 
         "temp": 0.3, 
         "atemp": 0.3,
         "hum": 0.3,
         "windspeed": 0.3 
       }
     ]
  }
}
```

A previsão gerada foi: 361.95

![Passo 18](./images/18.png)