# Projeto-Analise-de-dados-IMC-com-python
Este desafio busca aprofundar a análise dos dados gerados no [Simulacao-analise-de-dados-do-IMC](https://github.com/LucasLimaDevx/Simualacao-analise-de-dados-do-IMC), relacionando as variáveis IMC e problemas cardíacos com ferramentas estatísticas e de programação do curso de Forma Plena em Análise e Ciência de dados. 

## Tecnologias usadas
- Python
- Pandas
- Numpy
- Seaborn
- Matplotlib
  
## Problema proposto e os resultados obtidos
### 1.Para resolver, utilize o Python.

O IMC afeta a chance de ter problemas cardíacos? Vamos avaliar usando essa lógica:

- Separe os indivíduos do seu conjunto de dados em dois grupos: com e sem problemas cardíacos.

- Compare a média, mediana e desvio padrão do IMC nesses dois grupos.

- Geração de um gráfico de boxplot para visualizar diferenças. Com base no gráfico, há um padrão evidente? (coloque o gráfico aqui)

Medidas de posição obtidos:

![alt text](https://raw.githubusercontent.com/LucasLimaDevx/Projeto-Analise-de-dados-com-python/refs/heads/main/medias%20de%20cada%20grupo.png)

Boxplot:
![alt text](https://raw.githubusercontent.com/LucasLimaDevx/Projeto-Analise-de-dados-com-python/refs/heads/main/boxplot_distribui%C3%A7%C3%A3o_do_IMC_por_grupos.png)
O boxplot gerando nos mostra que um grupo de pessoas com o IMC alto, tendem a ter mais problemas cardíacos do que o grupo com IMC baixo.

### 2.Para resolver, utilize o Python.

Como os IMCs estão distribuídos?

- Crie um histograma da distribuição dos IMCs. Ele segue um formato simétrico ou há maior concentração em alguma faixa? (suba o histograma aqui)

- Compare a distribuição com as categorias da OMS: Abaixo do peso, Normal, Sobrepeso, Obesidade.

Histograma:
![alt text](https://raw.githubusercontent.com/LucasLimaDevx/Projeto-Analise-de-dados-com-python/refs/heads/main/histograma_imc.png) 

Podemos ver através do histograma que o grafíco tem uma curva assimetrica para a direita, onde boa parte da população deve ter um classificação de massa corporal entre peso-normalsobrepeso e obesidade grau de acordo com a OMS. O que implica também na presença com de um grupo de pessoa com IMC elevado para valores maiores 35.

### 3.Imagine que você trabalha como Cientista de Dados em um hospital e precisa desenvolver um sistema que ajude médicos a identificar pacientes em risco de problemas cardíacos com base no IMC. Se um paciente tem um IMC não exato (exemplo: 24.357896), qual conjunto numérico representa esse valor? O modelo precisa arredondar esse número? Justifique.

### Resultado
O melhor conjunto que pode representa um número com casas decimais é o conjunto dos números racionais através da divisão de dois números inteiros quaisquer. Para o caso do IMC não vale apena arredondar para o inteiro mais próximo mais alto ou mais baixo, mas diminuir o número de casas decimais ajudaria na visualização e padronização dos dados.

### 4.O conceito de módulo (valor absoluto) pode ser útil na análise do IMC? Como?

### Resultado
O valor absoluto é útil para obter valores positivos no cálculo da váriância para posteriomente calculamos o desvio padrão, pois sem isso os valores iriam se anular e não conseguiriamos transformar os valores elevados ao quadrado para a somatoria total da diferença para cada valor e a média para depois tiramos a raíz quadrada em seguida obtemos o quanto os valores desviam da média.
