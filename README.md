# 🎸 Classificador-de-instrumentos-musicais

Este projeto consiste em um classificador de imagens acessível via navegador, que possibilita aos usuários fazer o upload de imagens e classificá-las por meio de um modelo personalizado, treinado com o [Teachable Machine](https://teachablemachine.withgoogle.com/) . O aplicativo utiliza arquivos locais para carregar o modelo e realiza a inferência diretamente no navegador com o uso do [TensorFlow.js](https://www.tensorflow.org/js).

A execução desse projeto permite que usuário **enviar uma imagem de um instrumento musical** (piano, saxofone, guitarra, violão ou bateria) em seguida o sistema executa a classificação automaticamente de qual instrumento musical.

## 🔧 Ferramentas utilizadas

- HTML5; CSS3; TensorFlow.js; Teachable Machine; JavaScript.

## 🎼 Estrutura do Projeto

```bash
classificador-de-instrumentos-musicais/

├── index.html          # Página principal da aplicação
├── style.css           # Estilos da aplicação
├── script.js           # Lógica JavaScript
├── my_model/           # Pasta contendo o modelo treinado
│   ├── model.json      # Configuração do modelo
│   ├── metadata.json   # Metadados do modelo
│   └── weights.bin     # Pesos da rede neural
```

### 🪇 Pré-requisitos

- Navegador atual
- Editor de código 
- Modelo treinado com o Google Teachable Machine (arquivos model.json e metadata.json)

## 🪘 Funcionamento

1. **Inicialização do Modelo**: Assim que o aplicativo é iniciado, ele tenta carregar o modelo treinado em TensorFlow.js e seus metadados a partir da pasta model.

2. **Upload de Imagem**: O usuário pode enviar uma imagem tanto arrastando o arquivo para a interface quanto selecionando-o manualmente.

3. **Pré-processamento**: A imagem enviada é automaticamente redimensionada para 224x224 pixels e normalizada, garantindo compatibilidade com o formato de entrada esperado pelo modelo.

4. **Classificação**: O modelo analisa a imagem e calcula a probabilidade de pertencimento a cada uma das classes disponíveis.

5. **Visualização dos resultados**: Os resultados da classificação são exibidos em ordem decrescente de probabilidade, acompanhados de barras de progresso que indicam visualmente o nível de confiança do modelo.

## 🎵 Observações 

- Todo o processamento é realizado diretamente no navegador, sem que as imagens sejam enviadas para servidores externos
- O desempenho pode variar conforme as capacidades do dispositivo e o navegador em uso.
- Modelos com maior complexidade podem demandar mais tempo para serem carregados e processarem as imagens.


