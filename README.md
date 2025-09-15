# Classificação de Raças de Cachorros com Deep Learning

## Visão Geral
Este projeto utiliza técnicas de Deep Learning para desenvolver um classificador de raças de cachorros a partir de imagens. Implementado com a biblioteca FastAI e modelos de Deep Learning pré-treinados (ResNet34 e ResNet50), o sistema é capaz de identificar com alta precisão 25 raças diferentes de cachorros.

## Raças:
 american bulldog ,  american pit bull terrier ,  basset hound ,  beagle ,  boxer ,  chihuahua ,  english cocker spaniel ,  english setter ,  german shorthaired ,  great pyrenees ,  havanese ,  japanese chin ,  keeshond ,  leonberger ,  miniature pinscher ,  newfoundland ,  pomeranian ,  pug ,  saint bernard ,  samoyed ,  scottish terrier ,  shiba inu ,  staffordshire bull terrier ,  wheaten terrier ,  yorkshire terrier 

## Estrutura do Projeto
```
PUC_POS_DATA_SCIENCE/
├── MVP_03_DeepLearning.ipynb       # Notebook principal com todo o código
├── README.md                       # Este arquivo
```

## Funcionalidades Principais
- Classificação automática de 25 raças de cachorros
- Utilização de transfer learning com modelos ResNet34 e ResNet50
- Data augmentation para melhorar a generalização do modelo
- Análise detalhada de métricas e erros de classificação
- Comparação de desempenho entre diferentes arquiteturas de modelo

## Tecnologias Utilizadas
- **Python 3.x**: Linguagem de programação principal
- **FastAI 2.x**: Framework de alto nível para deep learning
- **PyTorch**: Framework de deep learning que serve como base para o FastAI
- **Jupyter Notebook**: Ambiente interativo para desenvolvimento e visualização
- **Google Colab**: Plataforma de execução com acesso a GPUs

## Principais Resultados
- **ResNet34**: Taxa de erro de aproximadamente 5.61% (acurácia de 94.39%)
- **ResNet50**: Taxa de erro de aproximadamente 3.71% (acurácia de 96.29%)
- Identificação de padrões de erro entre raças visualmente semelhantes
- Demonstração da eficácia do transfer learning mesmo com datasets relativamente pequenos

## Como Utilizar

### Pré-requisitos
- Python 3.6+
- Jupyter Notebook ou Google Colab
- Bibliotecas: fastai, fastbook, matplotlib

### Execução
1. Clone este repositório ou faça o download dos arquivos
2. Abra o notebook `MVP_03_DeepLearning.ipynb` no Jupyter ou no Google Colab
3. Execute todas as células sequencialmente
4. Os dados serão automaticamente baixados durante a execução
5. O modelo treinado pode ser exportado para uso posterior

### Predições com Novas Imagens
O notebook contém exemplos de como utilizar o modelo treinado para fazer predições em novas imagens, incluindo:
- Teste com imagens aleatórias do dataset
- Instruções para usar o modelo exportado

## Limitações e Trabalhos Futuros
- O modelo atual foi treinado com apenas 25 raças de cachorros
- Potencial para melhorias com:
  - Aumento do número de epochs de treinamento
  - Arquiteturas mais avançadas como EfficientNet
  - Expansão do dataset com mais imagens e raças
  - Técnicas adicionais de data augmentation
  - Ensemble de modelos

## Recursos Computacionais
- GPU: Disponível no Google Colab
- Tempo de treinamento: ~4 minutos para ResNet34, ~6 minutos para ResNet50
- Memória utilizada: ~1.5GB RAM


## Licença
Este projeto é destinado a fins educacionais e acadêmicos.

## Agradecimentos
- Dataset: [Oxford-IIIT Pet Dataset](https://www.robots.ox.ac.uk/~vgg/data/pets/)
- FastAI: Por fornecer ferramentas poderosas e intuitivas para deep learning
