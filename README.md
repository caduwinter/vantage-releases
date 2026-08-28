# Vantage

Compartilhe sua tela com áudio em 60fps pela Radmin VPN ou pela rede local,
com atraso baixo o suficiente para assistir junto sem incomodar.

## Instalar (recomendado): atualiza sozinho para sempre

Abra o menu Iniciar, digite **PowerShell**, abra e cole esta linha inteira:

```powershell
curl.exe -L -o "$env:TEMP\VantageSetup.exe" https://github.com/caduwinter/vantage-releases/releases/latest/download/Vantage-Setup.exe; Start-Process "$env:TEMP\VantageSetup.exe"
```

Instala em segundos, sem perguntas e sem pedir administrador. Daqui em
diante o app baixa as versões novas sozinho, em segundo plano, e mostra um
aviso discreto de **Atualizar** quando estiver pronta: um clique e acabou.
Nunca mais zip, nunca mais trocar pasta.

Sem aviso do Windows: o alerta só existe para arquivos baixados pelo
navegador, que ganham uma marca de origem; por este comando a marca não
existe. (Baixando o Setup pelo navegador o aviso pode aparecer; o passo a
passo para ele está mais abaixo.)

[Baixar o instalador pelo navegador](https://github.com/caduwinter/vantage-releases/releases/latest/download/Vantage-Setup.exe)

## Versão portátil (zip, sem atualização automática)

### [Vantage-1.15.0-win-x64.zip](https://github.com/caduwinter/vantage-releases/releases/download/v1.15.0/Vantage-1.15.0-win-x64.zip)

Versão 1.15.0 · Windows 64 bits · extrai e roda, mas cada versão nova é manual

## Se o navegador ou o Windows avisarem no download

O aviso aparece para qualquer programa novo que não paga por uma assinatura
digital, e não é uma detecção de vírus: cada zip é escaneado com o Windows
Defender antes de ser publicado e sai limpo. O alerta desaparece sozinho
conforme o arquivo ganha reputação.

- No Chrome ou Edge: clique nos três pontos do download, depois em
  **Manter** e **Manter mesmo assim**.
- Se abrir o exe e aparecer "O Windows protegeu seu PC": clique em
  **Mais informações** e depois **Executar assim mesmo**.

Regra de ouro: só baixe o Vantage desta página. Quem quiser conferir por
conta própria pode enviar o zip no [virustotal.com](https://virustotal.com)
antes de abrir.

## Primeira vez

1. Extraia a pasta do zip e abra `Vantage.exe`.
2. Clique em **Configurar agora**. O Windows pede permissão de administrador
   uma única vez, para liberar o app no firewall e ativar o áudio.
3. Copie o seu IP da Radmin, que aparece no topo da tela, e mande para os
   seus amigos. Adicione o IP deles no botão de mais.

## No dia a dia

Deixe o app aberto. Quando alguém da sua lista começar a transmitir, o nome
fica marcado como ao vivo e basta clicar em Entrar. Se ninguém estiver
transmitindo, o botão principal vira Transmitir.

Quem preferir não baixar nada consegue assistir pelo navegador, no endereço
`http://IP-DO-HOST:8080/`. Funciona no celular também.

## Se algo der errado

**Travando ou engasgando.** Na tela de transmitir, baixe a qualidade para
Leve e a resolução para 720p. Dá para mexer nisso com a transmissão no ar.

**Sem som.** No modo Nativo o áudio depende do filtro que a configuração
inicial registra. Se você pulou esse passo, o próprio app oferece ativar.

**Amigo não aparece.** Confira se os dois estão na mesma rede da Radmin e se
o IP salvo é o que aparece no topo da tela dele.

---

[Todas as versões](../../releases)
