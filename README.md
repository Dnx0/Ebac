# Módulo 18 - Análise do Preço da Gasolina com Pandas e Seaborn

Este projeto faz parte do Módulo 18 do curso de Análise de Dados da EBAC, com o professor André Peres. O objetivo é desenvolver uma análise visual da variação do preço da gasolina ao longo do tempo, utilizando a biblioteca `Pandas` para manipulação dos dados e `Seaborn` para criação de gráficos. O gráfico gerado é salvo como uma imagem PNG.

## Descrição

O projeto carrega uma base de dados de preços de gasolina no formato CSV, processa-a e cria um gráfico de linha para representar a variação dos preços ao longo do tempo. Essa visualização permite entender como o preço da gasolina se comporta, facilitando a análise e tomada de decisões.

## Requisitos

- Python 3.x
- Pandas
- Seaborn
- Matplotlib

## Como Utilizar

1. **Instale as dependências**:
   ```bash
   pip install pandas seaborn matplotlib

   Execute o código:

Salve o código a seguir em um arquivo Python, na mesma pasta que o arquivo gasolina.csv.
python
Copiar código
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt

# Carregando os dados do arquivo gasolina.csv
df = pd.read_csv('gasolina.csv')

# Criando o gráfico de linha
plt.figure(figsize=(10, 6))
sns.lineplot(data=df, x='dia', y='venda', marker='o')

# Adicionando título e rótulos dos eixos
plt.title('Preço da Gasolina ao Longo do Tempo')
plt.xlabel('Dia')
plt.ylabel('Preço (R$)')

# Salvando o gráfico como gasolina.png
plt.savefig('gasolina.png')

# Exibindo o gráfico
plt.show()
Visualize o Gráfico:

Após executar o código, o gráfico será salvo como gasolina.png no diretório do projeto e exibido na tela.
Estrutura do Projeto
gasolina.csv: Arquivo CSV contendo os dados de preço da gasolina por dia.
script.py: Código em Python para carregar, processar e visualizar os dados.
gasolina.png: Gráfico gerado mostrando a variação do preço da gasolina ao longo do tempo.
Exemplo do Gráfico Gerado


Este projeto foi desenvolvido no módulo 18 do curso de Análise de Dados da EBAC, com a orientação do professor André Peres.



Esse README inclui instruções de uso, dependências e uma descrição clara pa
