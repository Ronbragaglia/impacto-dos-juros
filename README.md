Descrição do Projeto:
Este projeto é uma Calculadora de Financiamento desenvolvida em Python, que permite calcular as parcelas e o total pago em financiamentos com diferentes taxas de juros. O código demonstra como calcular pagamentos mensais utilizando a fórmula de amortização de empréstimos, facilitando a compreensão do impacto das taxas de juros sobre o valor total a ser pago.

Funcionalidades:
Cálculo de Parcelas Mensais: Calcula o valor das parcelas mensais para diferentes taxas de juros.
Comparação de Cenários: Permite comparar o total pago em financiamentos com diferentes taxas de juros.
Fácil Ajuste de Parâmetros: Usuário pode facilmente ajustar o valor presente (PV), número de parcelas (n) e as taxas de juros para simular diferentes cenários.

Tecnologias Utilizadas:
Python: Linguagem de programação principal utilizada para desenvolver a calculadora.
Matemática Financeira: Aplicação de fórmulas financeiras para cálculo de parcelas e total pago.

Observações Detalhadas sobre o Código
Objetivo do Código:

O código calcula as parcelas mensais e o total pago em financiamentos com duas taxas de juros diferentes: 10% e 11.5% ao ano.
Utiliza a fórmula de amortização de empréstimos para calcular o valor da parcela mensal.

Parâmetros Utilizados:

PV: Valor presente do financiamento (R$ 750.000).
n: Número total de parcelas (420 meses, equivalente a 35 anos).
taxa_juros_10 e taxa_juros_115: Taxas de juros anuais convertidas para taxas mensais.

Função calcular_parcela:

Recebe o valor presente (PV), a taxa de juros mensal (i) e o número de parcelas (n).
Calcula o valor da parcela mensal (PMT) utilizando a fórmula:
𝑃
𝑀
𝑇
=
𝑃
𝑉
×
𝑖
1
−
(
1
+
𝑖
)
−
𝑛
PMT=PV× 
1−(1+i) 
−n
 
i
​
Retorna o valor da parcela mensal.

Cálculos Realizados:

Calcula as parcelas mensais para ambas as taxas de juros.
Calcula o total pago ao final do financiamento multiplicando a parcela mensal pelo número de parcelas.
Imprime os resultados formatados em reais.
Tecnologias e Conceitos Envolvidos:

Python: Linguagem de programação utilizada para implementar os cálculos.
Matemática Financeira: Aplicação da fórmula de amortização para cálculo de parcelas de empréstimos.
Programação Modular: Uso de funções para organizar o código de forma clara e reutilizável.
Pontos Positivos:

Clareza: O código é simples e direto, facilitando a compreensão.
Reutilização: A função calcular_parcela pode ser reutilizada para outros cálculos de financiamento.
Documentação: Comentários e docstrings estão presentes para explicar o funcionamento do código.
Possíveis Melhorias:

Entrada de Dados pelo Usuário: Permitir que o usuário insira os parâmetros (PV, n, taxa de juros) via entrada de teclado.
Validação de Dados: Adicionar verificações para garantir que os valores inseridos sejam válidos (por exemplo, não permitir taxas de juros negativas).
Interface Gráfica: Implementar uma interface gráfica simples para facilitar o uso.
Exportação de Resultados: Permitir a exportação dos resultados para um arquivo (como CSV ou Excel) para análises futuras.
Suporte a Diferentes Fórmulas: Implementar diferentes métodos de cálculo, como juros simples ou compostos, dependendo das necessidades do usuário.
Testes Automatizados: Adicionar testes unitários para garantir a precisão dos cálculos.
Boas Práticas Adotadas:

Uso de Funções: A função calcular_parcela torna o código modular e reutilizável.
Comentários e Docstrings: Melhoram a legibilidade e a manutenção do código.
Formatação de Saída: Utilização de f-strings para uma apresentação clara dos resultados.
