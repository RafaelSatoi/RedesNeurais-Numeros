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

## Como Testar
* Baixe o arquivo Nome_Do_Seu_Arquivo.xlsm presente neste repositório.
* Abra o arquivo no Microsoft Excel.
* Certifique-se de Habilitar Macros quando o Excel solicitar (necessário para a execução do código VBA).
* Vá até a aba do projeto, utilize a ferramenta de desenho e veja a mágica acontecer!
