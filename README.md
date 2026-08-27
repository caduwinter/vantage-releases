# Vantage

Compartilhe sua tela com áudio em 60fps pela Radmin VPN ou pela rede local,
com atraso baixo o suficiente para assistir junto sem incomodar.

## Instalar sem nenhum aviso (recomendado)

Abra o menu Iniciar, digite **PowerShell**, abra e cole esta linha inteira:

```powershell
curl.exe -L -o "$env:TEMP\vantage.zip" https://github.com/caduwinter/vantage-releases/releases/latest/download/Vantage-win-x64.zip; Expand-Archive -Force "$env:TEMP\vantage.zip" "$env:LOCALAPPDATA"; Start-Process "$env:LOCALAPPDATA\Vantage\Vantage.exe"
```

Ela baixa a versão mais nova, extrai e abre o app. Sem aviso nenhum: o
alerta do Windows só existe para arquivos baixados pelo navegador, que
ganham uma marca de origem; baixando por este comando a marca não existe.
Para atualizar depois, feche o Vantage e rode a mesma linha de novo.

## Ou baixar pelo navegador

### [Vantage-1.8.0-win-x64.zip](https://github.com/caduwinter/vantage-releases/releases/download/v1.8.0/Vantage-1.8.0-win-x64.zip)

Versão 1.8.0 · Windows 64 bits · não precisa instalar

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
