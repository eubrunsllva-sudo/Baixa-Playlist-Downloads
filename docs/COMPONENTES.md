# Componentes de terceiros

O Baixa Playlist integra os projetos abaixo. Consulte as páginas oficiais para obter os termos e avisos de cada versão incluída. A lista não substitui a revisão das licenças dos arquivos efetivamente distribuídos.

- [yt-dlp](https://github.com/yt-dlp/yt-dlp) — obtenção de informações e transferência de mídia.
- [Deno](https://github.com/denoland/deno) — runtime JavaScript usado pelo yt-dlp.
- [FFmpeg builds do projeto yt-dlp](https://github.com/yt-dlp/FFmpeg-Builds) — conversão e extração de áudio.
- [Electron](https://github.com/electron/electron) — aplicativo desktop.
- [electron-builder](https://github.com/electron-userland/electron-builder) — geração do instalador Windows.
- [React](https://github.com/facebook/react) e [Vite](https://github.com/vitejs/vite) — interface e compilação.

O script `npm run prepare:tools` consulta os releases oficiais e baixa os artefatos atuais para Windows x64. Assim, uma compilação futura pode incluir versões diferentes das usadas para gerar o instalador publicado. Para builds reproduzíveis, fixe versões e valide hashes, avisos de copyright e obrigações de redistribuição.

O pacote também inclui o plugin [yt-dlp-ChromeCookieUnlock](https://github.com/seproDev/yt-dlp-ChromeCookieUnlock), sob licença MIT, para lidar com bancos de cookies Chromium bloqueados no Windows. Ao usar Chrome ou Edge, o aplicativo pede confirmação antes de uma tentativa que pode fechar o navegador para liberar o arquivo.
