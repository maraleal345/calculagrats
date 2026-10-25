# Calculadora de Gratuidades (APK)

App que lê a foto da filipeta com o Gemini (`gemini-3.5-flash-lite`) e calcula o valor das gratuidades.

## Estrutura
- `www/index.html`: o app (tela, leitura e cálculo)
- `assets/`: ícone (`icon.png`) e tela de abertura (`splash.png`) usados para gerar o APK
- `capacitor.config.json` e `package.json`: configuração do Capacitor
- `.github/workflows/build-apk.yml`: o GitHub gera o APK sozinho

## Como gerar o APK
1. Envie todos os arquivos desta pasta para um repositório no GitHub (branch `main`).
2. Abra a aba **Actions**. O fluxo **Gerar APK** roda sozinho a cada envio (ou clique em **Run workflow**).
3. Quando terminar (cerca de 5 a 8 minutos), abra a execução e baixe o arquivo **calculadora-gratuidades-apk** na seção *Artifacts*.
4. Extraia o zip e instale o `app-debug.apk` no celular (permita instalar de fontes desconhecidas).

## Chave da API do Gemini
O app pede a chave só na primeira abertura, testa, salva no aparelho e esconde o campo. A chave não fica no código.
