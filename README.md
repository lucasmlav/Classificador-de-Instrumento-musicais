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

## ▶️ Como rodar o projeto

> ⚠️ Este projeto **precisa ser executado em um servidor local via liver server**.

### ✅ Requisitos

- Navegador moderno (Chrome, Brave, Firefox...)
- Editor de código (VS Code recomendado)
- Extensão **Live Server** no VS Code

### 🧪 Passo a passo com Live Server (VS Code)

1. Clone o repositorio em sua maquina local.
2. Abra o VS Code e instale a extensão [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer)
3. Abra o repositorio pelo vscode e com liveserver ja instalado, selecione no canto inferior direito **"Go Live"**.
4. O navegador será aberto automaticamente e o sistema estará pronto para uso.
5. Envie uma imagem de roupa e clique em **"Classificar"** para ver o resultado.

### 🚫 Não funciona com duplo clique no `index.html`

Por segurança, navegadores modernos bloqueiam o acesso a arquivos locais via `file://`, impedindo que o modelo carregue corretamente.

Use sempre o Live Server para rodar o projeto localmente.
