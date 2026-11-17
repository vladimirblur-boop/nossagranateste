# Nossa Grana 0.4.8 — Preparação para instalação

A versão 0.4.8 adiciona os arquivos de PWA: manifest, ícones e service worker para funcionamento offline depois de instalado. O aplicativo continua local, sem autenticação ou sincronização. NÃO há servidor publicado neste pacote.

## Importante
Abrir `index.html` diretamente (`file://`) permite testar o protótipo, mas NÃO instala o PWA no iPhone. Para instalar no Android e iPhone, os arquivos precisam ser publicados em uma origem HTTPS estável. O mesmo endereço HTTPS deve ser mantido nas futuras atualizações para preservar o armazenamento local da origem. **Antes de mudar de `file://` para HTTPS, exporte backup JSON e importe no novo endereço.**

Nunca publique um backup JSON com seus dados financeiros. Publique somente os arquivos do aplicativo.

## Próximos passos
1. Fazer backup JSON no Chrome.
2. Publicar somente os arquivos deste pacote num site HTTPS de sua escolha.
3. Abrir o endereço no Android (Chrome > menu > Instalar aplicativo) e no iPhone (Safari > Compartilhar > Adicionar à Tela de Início).
4. Importar o backup no aparelho desejado, somente depois de confirmar que está no site correto e confiável.
5. Sincronização de casal ainda não implementada: **não importe dados reais em dois aparelhos esperando que se sincronizem**.

## Testes
`node testes-logica.js` testa regras de cálculo. A interface e a instalação precisam ser validadas em dispositivos reais.
