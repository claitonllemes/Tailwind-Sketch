# Tailwind Colors Sketch Plugin

Plugin do Sketch para importar cores do Tailwind CSS 4.

## Instalação

1. Baixe a última versão na aba [Releases](../../releases).
2. Descompacte e dê um duplo clique no arquivo `.sketchplugin`.

## Desenvolvimento

### Requisitos

- Node.js ou Bun
- Sketch

### Comandos

- `npm run build`: Compila o plugin.
- `npm run release`: Prepara uma nova versão para lançamento (build + zip + update appcast).

## Publicação (Release)

Para lançar uma nova versão com atualizações automáticas:

1. Atualize a versão no `package.json`.
2. Configure seu usuário e repositório GitHub em:
   - `build.js` (campo `appcast`)
   - `.appcast.json` (campo `downloadURL`)
3. Execute o comando de release:
   ```bash
   npm run release
   # ou
   bun run release
   ```
4. Commit e Push das alterações (incluindo o `.appcast.json` atualizado):
   ```bash
   git add .
   git commit -m "Release v1.0.1"
   git push
   ```
5. Crie uma **Release** no GitHub:
   - Tag: `v1.0.1` (mesma versão do package.json)
   - Título: `v1.0.1`
   - Anexe o arquivo `.zip` gerado na pasta do projeto.

O Sketch verificará automaticamente o arquivo `.appcast.json` no branch `main` para notificar os usuários sobre a atualização.
