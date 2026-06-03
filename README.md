# Rede Neural - Números

Este projeto consiste no desenvolvimento autoral de uma Rede Neural Artificial Multicamadas (MLP) criada inteiramente do zero dentro do Microsoft Excel utilizando VBA (Visual Basic for Applications), sem o uso de qualquer biblioteca externa de Machine Learning.
O objetivo principal foi consolidar o entendimento prático e matemático dos algoritmos fundamentais de Deep Learning (Álgebra Linear, Cálculo e Otimização).

## Como Funciona?
O projeto utiliza o recurso de desenho nativo do Excel (Draw) como interface de entrada de dados:
1. O usuário desenha um número de 0 a 9 livremente na tela.
2. O desenho é convertido em uma matriz de pixels e alimentado na rede neural.
3. A rede processa os dados através das camadas ocultas e exibe o número identificado na planilha em tempo real.

## Detalhes Técnicos & Dataset Autoral
* Arquitetura: Rede Neural Feedforward Multicamadas (Multi-Layer Perceptron).
* Algoritmos: Implementação manual dos processos de Forward Propagation e Backpropagation (cálculo de gradientes e atualização de pesos via gradiente descendente).
* Dataset 100% Autoral (Construído do Zero): Em vez de utilizar as 60.000 imagens prontas do dataset MNIST tradicional, o modelo foi treinado utilizando um conjunto enxuto de 200 desenhos próprios coletados diretamente na interface do Excel.

## Pré-requisitos
* Baixe o arquivo Numeros.xlsm presente neste repositório.
* Abra o arquivo no Microsoft Excel.
* Certifique-se de Habilitar Macros quando o Excel solicitar (necessário para a execução do código VBA).

## Parâmetros de Configuração
Antes de rodar o modelo, você pode ajustar os hiperparâmetros da rede diretamente na planilha para testar diferentes cenários de convergência:
* Camada Oculta: Define a quantidade de neurônios na camada intermediária da rede.
* Learning Rate (Taxa de Aprendizado): Controla o tamanho dos passos na atualização dos pesos durante o gradiente descendente.
* Max Épocas: Estipula o número máximo de iterações que o algoritmo executará durante o treinamento.

## Interface e Controles (Botões)
O controle do fluxo é feito através dos seguintes botões:
* Banco de Dados: Converte o seu desenho atual em uma matriz de dados e o armazena no banco de dados local da planilha para ser usado no treino.
* Nova Rede: Reinicia completamente a estrutura, zerando e gerando novos pesos e biases de forma aleatória.
* Treino: Inicia o algoritmo de backpropagation do absoluto zero, utilizando todos os desenhos armazenados no seu banco local até que o modelo convirja.
* Adivinhar: Faz o forward pass do seu desenho atual através da rede treinada, calculando as probabilidades e devolvendo o dígito identificado em tempo real.
