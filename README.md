# Narrador Studio 🎙️

Aplicativo independente para gerar narrações usando ElevenLabs e importar áudios externos.

## Recursos
- Texto para voz via ElevenLabs
- Busca de vozes da conta
- Modelos Multilingual v2, v3 e Flash v2.5
- Ajustes de estabilidade e similaridade
- Preview e download em MP3
- Importação de arquivos de áudio e biblioteca temporária local
- Interface responsiva em português

## Como abrir
O projeto é uma página web estática. Abra `index.html` em um navegador moderno.

## Publicar com GitHub Pages
1. Entre no repositório **GitRegis**.
2. Abra **Settings → Pages**.
3. Em **Build and deployment**, escolha **Deploy from a branch**.
4. Branch: `main`; pasta: `/ (root)`; clique **Save**.
5. Aguarde o GitHub Pages publicar o site. A URL aparecerá na mesma tela.

## Como usar
1. Abra o site.
2. Cole sua chave API ElevenLabs no campo da chave. A chave não é salva pelo app.
3. Clique em **Buscar vozes da conta** e selecione uma voz.
4. Selecione o modelo e cole o texto.
5. Clique **Gerar áudio**, ouça e baixe o MP3.
6. Para áudio externo, use o seletor em **Áudios externos**. Arquivos importados ficam apenas na memória do navegador durante a sessão.

## Segurança
- **Nunca** coloque sua chave API dentro de arquivos do repositório, em código ou screenshots.
- A chave é digitada na página e enviada diretamente ao serviço ElevenLabs no navegador; não é persistida no site.
- Se o navegador bloquear a conexão por CORS, a versão estática não poderá fazer a requisição. Nesse caso, será necessário adicionar um pequeno backend seguro (por exemplo, uma função serverless) para intermediar a API.
- Publicar no GitHub Pages deixa o código do site publicamente acessível. Não publique uma chave, mesmo em repositório privado como medida de segurança.

## Limitações desta primeira versão
- Biblioteca não persiste depois que fechar/recarregar a página.
- Não inclui editor de áudio/cortes; permite importar, ouvir e baixar.
- O processamento de texto e áudio depende da conta e dos limites da ElevenLabs.

