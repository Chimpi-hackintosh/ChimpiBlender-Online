# Aviso de suporte e atualizações

## Política

A partir de **04/11/2026 às 00h UTC**, versões abaixo da mínima declarada deixam de receber correções de segurança do proprietário

Antes dessa data o aviso informa que o suporte está prestes a terminar — depois informa que as atualizações de segurança terminaram

O texto explica o risco de falhas sem afirmar que o usuário ou o aplicativo já foi infectado

| Projeto | Publicação conferida em 11/11/2026 | Classificação | Versão mínima sustentada |
| --- | --- | --- | --- |
| OpenCore Helper | [v3.0.2](https://github.com/Chimpi-hackintosh/OpenCore-Helper/releases/tag/v3.0.2) | Estável | 3.0.2 |
| SnoopyOS Lite | [v0.1-lite.3](https://github.com/Chimpi-hackintosh/SnoopyOS-Image/releases/tag/v0.1-lite.3) | Prévia · edição Lite | 0.1.3 |
| SnoopyOS Games | [v0.2-games.1](https://github.com/Chimpi-hackintosh/SnoopyOS-Image/releases/tag/v0.2-games.1) | Prévia · edição Games | 0.2.1 |
| ChimpiAI | [v1.1.0](https://github.com/Chimpi-hackintosh/ChimpiAI/releases/tag/v1.1.0) | Estável | 1.1.0 |
| WinSIMU | [v0.1.0-alpha](https://github.com/Chimpi-hackintosh/WinSIMU/releases/tag/v0.1.0-alpha) | Prévia · alpha | 0.1.0-alpha |
| ChimpiCode | [v1.1.0-preview.3](https://github.com/Chimpi-hackintosh/ChimpiCode/releases/tag/v1.1.0-preview.3) | Prévia | 1.1.0-preview.3 |
| ChimpiBridge | [v0.1.1](https://github.com/Chimpi-hackintosh/ChimpiBridge/releases/tag/v0.1.1) | Prévia | 0.1.1 |
| ChimpiShare | [v0.1.0](https://github.com/Chimpi-hackintosh/ChimpiShare/releases/tag/v0.1.0) | Prévia | 0.1.0 |
| ChimpiConstruções | Sem Release para download | Código-fonte, sem binário | Sem mínimo publicado |
| ChimpiBlender Online | Site, sem Release de aplicativo | Site; implantação desta tabela ainda não confirmada | Revisão web 20261102, não é versão de app |
| ChimpiNotch | [v1.0.4](https://github.com/Chimpi-hackintosh/ChimpiNotch/releases/tag/v1.0.4) | Estável | 1.0.4 |
| Chimpi3D | [v0.3.1-build-11](https://github.com/Chimpi-hackintosh/Chimpi3D-Installer/releases/tag/v0.3.1-build-11) | Estável | 0.3.1 |
| ChimpiNFC | [v0.1.0-build-2](https://github.com/Chimpi-hackintosh/ChimpiNFC/releases/tag/v0.1.0-build-2) | Prévia | 0.1.0 |
| Chimpi Find My Kids | [v1.3.1-preview.1](https://github.com/Chimpi-hackintosh/Chimpi-Find-My-Kids/releases/tag/v1.3.1-preview.1) | Prévia | 1.3.1-preview.1 |
| Chimpi Parents Find My Kids | [v1.3.1-preview.1](https://github.com/Chimpi-hackintosh/Chimpi-Parents-Find-My-Kids/releases/tag/v1.3.1-preview.1) | Prévia | 1.3.1-preview.1 |
| Earth-Blender | Sem Release para download | Código-fonte, sem binário | Sem mínimo publicado |
| ChimpiBypass | Sem Release para download | Código-fonte, sem binário | Sem mínimo publicado |
| ChimpiNature | [v1.0.0](https://github.com/Chimpi-hackintosh/ChimpiNature/releases/tag/v1.0.0) | Prévia | 1.0.0 |

Observação: o PR de ChimpiConstruções menciona uma PWA externa, mas o PR ainda está aberto e a disponibilidade do endereço não foi confirmada nesta revisão — por isso o catálogo mantém o projeto como código-fonte sem Release para download, sem classificá-lo como site publicado

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

O catálogo público contém 18 entradas correspondentes a 17 repositórios públicos, porque SnoopyOS Lite e Games são edições separadas; não inclui o repositório privado

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


## Releases públicas conferidas em 11/11/2026

Os mínimos de WinSIMU e ChimpiCode preservam os identificadores `alpha` e `preview.3` das únicas Releases publicadas dessas linhas — não há uma Release estável `0.1.0` ou `1.1.0` para esses projetos

A Release estável `v1.1.0` do ChimpiAI foi conferida com o instalador Windows publicado e seu digest SHA-256 informado pelo GitHub — a disponibilidade no catálogo WinGet continua dependendo da aprovação externa descrita pelo projeto

A Release `v1.0.0` do ChimpiNature foi conferida como prévia, com JAR do mod Fabric e shaderpack opcional publicados — o projeto informa que ainda precisa de validação dentro do Minecraft real

## Entrada pública removida em 08/11/2026

O ChimpiKids deixou de aparecer na paginação autorizada e a consulta direta ao repositório passou a retornar `404` — a entrada foi removida do catálogo porque a Release não pôde mais ser verificada, sem afirmar se o repositório foi excluído ou se o acesso mudou
