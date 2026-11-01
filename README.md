# Baixa Playlist

Aplicativo para Windows que organiza downloads em lote de áudio de vídeos ou playlists do YouTube e YouTube Music, convertendo o conteúdo para MP3. Use somente conteúdo que você criou ou tem autorização para salvar. O aplicativo não remove DRM nem contorna controles de acesso.

## Baixar e instalar

**Requer administrador:** no Windows, clique com o botão direito no instalador e escolha **Executar como administrador**. Sem elevação, o aplicativo não será instalado. Baixe o instalador para Windows x64 na página [Releases](https://github.com/eubrunsllva-sudo/Baixa-Playlist-Downloads/releases). Não é necessário instalar Python, Node.js ou FFmpeg no computador de destino.

Veja o [Guia de instalação](docs/INSTALACAO.md) e o [Guia de uso](docs/USO.md).

## Recursos

- Baixa uma faixa ou uma playlist completa.
- Detecta automaticamente se o link aponta para um vídeo ou playlist; também permite escolher o modo manualmente.
- Converte o áudio para MP3 com opções de 128, 192, 256, 320 kbps ou melhor qualidade disponível.
- Permite escolher a pasta de destino e acompanha as mensagens e o progresso.
- Pode usar cookies de uma sessão local do Firefox quando o usuário está autorizado a acessar o conteúdo.
- Inclui yt-dlp, Deno e FFmpeg no instalador.

A qualidade selecionada não pode superar a qualidade da fonte original. A disponibilidade depende do conteúdo, da rede e das regras de acesso do YouTube.

## Requisitos

Para instalar: Windows 10 ou 11 de 64 bits e conexão com a internet para baixar conteúdo. Para desenvolver ou gerar o instalador: Windows x64, Node.js LTS, npm e conexão com a internet.

## Desenvolvimento

```powershell
npm install
npm run dev
```

Para gerar o instalador no Windows x64:

```powershell
npm run dist:win
```

Esse comando baixa as ferramentas necessárias para `tools/`, compila o aplicativo e cria o instalador em `release/`. Consulte [Desenvolvimento e compilação](docs/DESENVOLVIMENTO.md).

## Componentes de terceiros

O aplicativo usa Electron, React, Vite, yt-dlp, Deno e FFmpeg. Consulte [Fontes e licenças](docs/COMPONENTES.md) e os termos dos respectivos projetos antes de redistribuir versões modificadas.

## Ajuda

Se um download falhar, expanda **Atividade** no aplicativo e inclua as mensagens exibidas ao relatar o problema. Não compartilhe cookies, senhas nem arquivos de perfil do navegador.
