# Oh-My-Posh
## Este repositório é sobre a personalização do Terminal no Windows 11 para o pessoal que gosta de personalizar o seu terminal.
_Aqui, indicarei as referências que usei para dar crédito ao trabalho de uma pesquisa mais abrangente e fornecer alguns detalhes para quem é leigo no assunto._

_O processo é simples e direto._

**Após a instalação do PowerShell, aplicativo disponível na loja da MS, é necessário executar `winget install JanDeDobbeleer.OhMyPosh` no terminal e após o termino do processo de instalação, reiniciar o terminal.**

> Abre o arquivo *Microsoft.PowerShell_profile.ps1* (para localizar ele, no terminal digite: `echo $PROFILE`).
>
> Podes digitar `code $PROFILE` se tiveres o VS Code na sua máquina.
>
>  Depois deves digitar os comandos que apontam onde sua configuração `.json` está, algo como `oh-my-posh --init --shell pwsh --config C:/LOCAL/DO/ARQUIVO/ohmyposh.json | Invoke-Expression`

_A configuração que cobre uma necessidade significativa é a seguinte:_


```json
{
  "segments": [
    {
      "type": "git",
      "style": "powerline",
      "powerline_symbol": "",
      "foreground": "#ffffff",
      "background": "#ff0000",
      "properties": {
        "display_status": true,
        "display_stash_count": true
      }
    }
  ]
}
``` 


[A referência geral](https://www.hanselman.com/blog/my-ultimate-powershell-prompt-with-oh-my-posh-and-the-windows-terminal)
