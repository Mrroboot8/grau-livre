# Grau Livre 3D: como gerar o APK

Você precisa de uma conta no GitHub (grátis). Dá para fazer tudo pelo celular.

1. Crie um repositório novo no GitHub, por exemplo `grau-livre`.
2. Envie todo o conteúdo desta pasta para o repositório, mantendo as pastas `www` e `.github/workflows`.
   No site do GitHub: Add file, Upload files. Pelo celular, descompacte o zip antes.
3. Abra a aba **Actions**. O fluxo "Gerar APK" roda sozinho. Se não rodar, abra ele e toque em **Run workflow**.
4. Espere uns 5 a 10 minutos. Quando ficar verde, abra a execução e baixe o arquivo `grau-livre-apk` em **Artifacts**.
5. Descompacte, abra o `app-debug.apk` no celular e permita instalar de fontes desconhecidas quando o Android pedir.

## Observações

- O APK sai em modo debug, bom para testar e jogar. Para publicar na Play Store é preciso gerar uma versão assinada (AAB).
- O jogo fica na pasta `www`. Mudou o jogo, é só enviar o novo `www/index.html` e o APK é gerado de novo.
- A fonte do título é baixada da internet. Sem internet o jogo usa uma fonte padrão e continua funcionando.
- O nome do app é `Grau Livre` e o identificador é `com.grau.livre`. Para trocar, edite `capacitor.config.json`.
