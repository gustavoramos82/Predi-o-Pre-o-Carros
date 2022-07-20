# Predição nos Preço dos Carros

Neste Projeto, a partir de um dataset obtido no kaggle (que pode ser obtido [aqui](https://www.kaggle.com/datasets/deepcontractor/car-price-prediction-challenge)), no qual vai ser feito análise exploratória, tratamento dos dados e modelagem e verificar qual modelo vai ter a melhor perfomace com base nas métricas.

## Análise Exploratŕia dos Dados

![image](https://user-images.githubusercontent.com/39843884/179794788-7016712f-b942-4861-9c9c-bcbc0b47e805.png)

O dataset é composto de 19237 linhas e 18 colunas e verificando a distribuição dos preços foi verificaso um *outlier* que não ia permitir fazer uma análise acerca do preço, então o mesmo foi retirado (como pode ser visto na figura abaixo).

![image](https://user-images.githubusercontent.com/39843884/179795702-5b71f9ef-4707-4085-a321-7b85a9742122.png)

Tirando o *outlier* deu pra ter uma melhor visão acercar dos preços dos carros.

![image](https://user-images.githubusercontent.com/39843884/179796093-2826007b-29ce-4219-8119-9d0523a2bceb.png)

Podemos ver que a maioria dos valores está entre 0 e 50 mil, sedo que em torno de mil que temos em maior quantidade.

![image](https://user-images.githubusercontent.com/39843884/179797101-3a4efadf-a96c-429b-a595-0e0a0af9566f.png)

Os maiores fabricantes estão Hyundai e Toyota, com um pouco mais de 3500.

![image](https://user-images.githubusercontent.com/39843884/179797337-5711d6dd-db07-4fd0-a76b-003a0da89f2e.png)

Podemos ver que marcas como Peugeut, Uaz e Haval costuma ter preços mais baratos em comparação por exemplo de Bentley que costuma ter carros mais baratos

![image](https://user-images.githubusercontent.com/39843884/179797522-21077b12-c12c-48d0-a45d-67c4d1db005d.png)

Quanto ao preço dos carros, vemos que a maioria foi construida entre 2010 e 2020.

![image](https://user-images.githubusercontent.com/39843884/179797654-e642a471-589d-4b76-a16b-709ff8228693.png)

A maioria dos carros tem couro em seu interior, e a partir de 100 mil, temos q uma grande parte dos carros tem couro em seu interior.

![image](https://user-images.githubusercontent.com/39843884/179797808-f5c12b9b-1b32-4ed2-9ef8-831864ac058a.png)

Uma grande parte dos carros tem quatro carros, em uma quantidade muito discrepante, se comparada aos outros, logo o mesmo vai ser desconsiderado na etapa de modelagem, para que o modelo não se influencie por esses valores, o mesmo occore com o que direção fica o lado do motorista em qua uma grande parte é do lado esquerdo e o tipo de caixa de engrenagem em que a maioria é automático.
![image](https://user-images.githubusercontent.com/39843884/179798301-918aac2c-630d-4aa5-9847-b1247f5ffa8a.png)![image](https://user-images.githubusercontent.com/39843884/179798515-bcce9ba5-399b-4015-9bc2-71a2022abd5c.png)

Quanto, ao combustivel, o mais utilizado é a gasolina

![image](https://user-images.githubusercontent.com/39843884/179798926-5ed527e2-e0f0-498a-80bd-841095ec6a8b.png)

Podemos ver que a maioria dos carros tem 4 e 12 airbaigs, e em relação ao preço com 14 e 15 e 11, tem-se um preço menor se comparado a 0, 4, 10 e 14.

![image](https://user-images.githubusercontent.com/39843884/179799310-62b2f904-016e-445d-9ddc-63820e3fc7d4.png)

E os três modelo que mais se tem são Prius, Sonata e Camry

![image](https://user-images.githubusercontent.com/39843884/179799433-8d6855cc-bfb7-4613-80e1-d3c4be40d2b8.png)


## Modelagem

Foi aplicados os tratamentos e foi aplicados modelos de machine learning, em que o dataset foi dividido em 80% de treino e 20% de teste, a que teve melhor perfomace foi o *random forest* com as eguintes métricas:

![image](https://user-images.githubusercontent.com/39843884/179984799-ddd9eaba-612c-4fce-ad48-2c904d681583.png)


## Conclusão

Podemos ver que o modelo apesar de ter até uma boa métrica, pode ser melhorado com uma boa coleta de dados pois como pode ver o mesmo tem preços muito discrepante, o que contribue para que o modelo não tenha uma boa perfomace, como podemos ver no gráfico abaixo, abaixo de 5 mil até que o modelo tem uma boa perfomace, mas acima disso, o modelo não consegue fazer uma boa estimativa, mostrando que o modelo só serie eficiente para preços abaixo desse valor, acima disso teria que ter uma maior coleta de dados para melhorar a perfomace.

![image](https://user-images.githubusercontent.com/39843884/179985304-b64fc3f8-88cb-46cf-b410-5ca891bdbd6e.png)
