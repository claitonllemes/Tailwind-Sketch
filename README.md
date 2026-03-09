# Tailwind Colors Sketch Plugin

Plugin do Sketch para importar a paleta de cores completa do **Tailwind CSS 4**.

## ✨ Funcionalidades

- **Cores Oficiais do Tailwind 4**: Importa todas as cores, incluindo os novos tons e variações (Slate, Gray, Zinc, Neutral, Stone, Taupe, Mauve, Mist, Olive, etc.).
- **Conversão Automática**: Converte valores OKLCH nativos do Tailwind 4 para HEX, garantindo fidelidade visual no Sketch.
- **Organização**: Cria variáveis de cor organizadas por grupos e tonalidades (50 a 950).
- **Atualização Inteligente**: Preserva suas cores personalizadas e atualiza apenas as cores relacionadas ao Tailwind.

## 📦 Instalação

1. Baixe a versão mais recente na aba [Releases](https://github.com/claitonllemes/Sketch-Plugin/releases).
2. Descompacte o arquivo baixado.
3. Dê um duplo clique no arquivo `Tailwind Colors.sketchplugin` para instalar.

## 🚀 Como usar

1. Abra um documento no Sketch.
2. Acesse o menu **Plugins** > **Tailwind Colors** > **Importar Tailwind Colors**.
3. Ou use o atalho: `Ctrl` + `Shift` + `T`.
4. Pronto! As cores serão adicionadas ao seu documento.

> **💡 Nota:** O plugin detecta e atualiza apenas as cores do Tailwind, mantendo intactas quaisquer outras cores que você tenha criado no documento.

---

## 🛠 Desenvolvimento

Para contribuir ou modificar o plugin:

### Requisitos

- Node.js ou Bun
- Sketch (v70 ou superior)

### Comandos

- `npm run build`: Compila o plugin.
- `npm run release`: Gera uma nova versão (build + zip).

### Publicação

1. Atualize a versão no `package.json`.
2. Execute `npm run release`.
3. Faça commit das alterações (incluindo `.appcast.json`).
4. Crie uma Release no GitHub anexando o `.zip` gerado.
