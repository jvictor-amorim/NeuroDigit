# NeuroDigit

Rede neural multicamadas (MLP) desenvolvida em Python e TensorFlow para identificar dígitos manuscritos (0 a 9) utilizando o famoso dataset MNIST.

## 🧠 Sobre o Projeto

O projeto utiliza a biblioteca TensorFlow (versão 1.x) para construir e treinar uma Rede Neural Artificial capaz de classificar imagens de dígitos escritos à mão. O modelo possui uma camada de entrada para as imagens de 28x28 pixels, três camadas ocultas (com 512, 256 e 128 neurônios) e uma camada de saída com 10 classes (dígitos de 0 a 9).

O script também demonstra como carregar uma imagem externa (como `oito.png`), processá-la e realizar uma predição usando o modelo treinado.

## 🛠️ Tecnologias Utilizadas

- **Python**
- **TensorFlow** 1.4.0
- **NumPy** 1.14.3
- **Pillow** (PIL)

## ⚙️ Como Executar

### 1. Preparar o Ambiente

Recomenda-se o uso de um ambiente virtual (venv). Para instalar as dependências, execute:

```bash
pip install -r requirements.txt
```

### 2. Rodar o Modelo

Para treinar a rede neural e realizar a predição na imagem de teste (`oito.png`), execute o script principal:

```bash
python main.py
```

Durante a execução, o script irá:
1. Baixar o dataset MNIST (caso ainda não esteja baixado).
2. Treinar o modelo exibindo a perda (loss) e a acurácia a cada 100 iterações.
3. Exibir a acurácia final usando o conjunto de testes.
4. Ler o arquivo `oito.png` e informar qual número a rede neural identificou.

## 📁 Estrutura de Arquivos Principais

- `main.py`: Script principal com a lógica da rede neural, treinamento e validação.
- `requirements.txt`: Dependências necessárias para rodar o projeto.
- `oito.png` / `img_teste.png`: Imagens de teste para verificar a capacidade de generalização e predição do modelo treinado.
