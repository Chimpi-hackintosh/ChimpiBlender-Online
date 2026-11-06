# Aviso de suporte e atualizações

## Política

A partir de **04/11/2026 às 00h UTC**, versões abaixo da mínima declarada deixam de receber correções de segurança do proprietário

Antes dessa data o aviso informa que o suporte está prestes a terminar — depois informa que as atualizações de segurança terminaram

O texto explica o risco de falhas sem afirmar que o usuário ou o aplicativo já foi infectado

| Aplicativo | Versão ou publicação pública conferida em 06/11/2026 | Mínima |
| --- | --- | --- |
| ChimpiBlender Online | Site sem versão de Release | Ainda sem mínimo de versão publicado |
| Earth-Blender | Sem Release publicada | Ainda sem mínimo de versão publicado |
| ChimpiBypass | Sem Release publicada, apesar do artefato temporário do workflow | Ainda sem mínimo de versão publicado |
| Chimpi Find My Kids | v1.3.1-preview.1 | 1.3.1-preview.1 |
| Chimpi Parents Find My Kids | v1.3.1-preview.1 | 1.3.1-preview.1 |

## Comportamento

O campo opcional `windows_setup` registra o instalador do OpenCore Helper disponível no GitHub Releases. Ele vincula a tag ao SHA-256 do arquivo publicado e ao piso do fluxo assistido, Windows 11 x64 nativo (build 22000). Esse piso vale para a atualização assistida e não é uma declaração de compatibilidade de todos os pacotes

Ao revisar um novo lançamento, mantenha os metadados de instalação assistida vinculados ao instalador estável realmente publicado. Sem um instalador correspondente e requisitos verificados, o app mantém o aviso informativo

- Detecta o idioma do sistema ou navegador — português, inglês, espanhol, francês, alemão, italiano, russo, chinês, japonês, coreano, árabe e hindi, com inglês como alternativa
- Compara versões numericamente e, quando a mínima inclui uma prévia, também compara seus identificadores — `preview.0` fica abaixo de `preview.1` e uma versão estável equivalente fica acima da prévia
- Consulta somente dados públicos de suporte por HTTPS, com prazo limitado e catálogo local quando está sem internet
- Não envia arquivos, prompts, senhas, dados de hardware ou dados NFC
- Mostra a versão instalada e a mínima, com opções de atualizar, ver a tabela ou deixar para depois
- Abre a página oficial e preserva a decisão de baixar e instalar com o usuário

A tabela pública fica em [Apps e suporte](https://chimpi-hackintosh.github.io/ChimpiBlender-Online/support.html) depois que o PR do site for integrado e o Pages for publicado

## Distribuição e limites

**Alterar o repositório não altera binários já instalados** — versões antigas sem verificador precisam receber uma atualização manual inicial para passarem a consultar a política

Este PR entrega código e verificações — não equivale a um novo Release, atualização instalada ou site já implantado

As prévias continuam identificadas como prévias — os números da tabela vêm de lançamentos existentes e não foram inventados para esta alteração

O catálogo público inclui 17 entradas públicas verificadas em 06/11/2026 e não inclui repositórios privados

## Validação local desta alteração

`node --test tests/support.test.cjs`: 5 testes aprovados

Os testes do aviso cobrem versões iguais e mais novas sem alerta, versões antigas com alerta, mudança exata de data, traduções, falha de rede e rejeição de links não oficiais

A revisão interna do site `20261102` identifica esta geração do verificador — não representa uma versão de aplicativo já lançada

O catálogo permite comparar revisões do site em futuras implantações sem inventar versões semânticas de Releases


## Atualização das prévias 1.3.1

As Releases públicas `v1.3.1-preview.1` dos dois apps Find My Kids foram conferidas em 04/11/2026, incluindo os nomes dos APKs e os digests SHA-256 informados pelo GitHub

A mínima foi elevada somente depois da publicação dessas Releases e permanece marcada como prévia

## Projetos públicos adicionados em 06/11/2026

Earth-Blender e ChimpiBypass foram incluídos como projetos sem Release para download, sem versão mínima inventada

O workflow do ChimpiBypass gerou um artefato temporário com sucesso, mas isso não equivale a uma Release publicada nem comprova instalação ou funcionamento no computador do usuário
