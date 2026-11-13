# 🐒 ChimpiBlender Online

**Seu mini estúdio 3D no navegador, em português e sem instalação** 💜

O ChimpiBlender Online é um editor 3D leve, desenvolvido em **HTML, CSS e JavaScript puro**. Ele funciona sem bibliotecas externas e também pode ser aberto offline para modelos 3D

## 🌐 Acessar o editor

Quando o GitHub Pages estiver habilitado neste repositório, o site ficará disponível em:

`https://chimpi-hackintosh.github.io/ChimpiBlender-Online/`

**Antes da publicação:** abra `index.html` diretamente no navegador do computador ou use um servidor local para testar

## ✨ Funcionalidades

- Modelos 3D: cubo, esfera, cilindro, cone, rosca e plano
- Mover, girar, redimensionar, duplicar, excluir e colorir objetos
- Câmera orbital com zoom, panorâmica e foco
- Desfazer/refazer e rascunho salvo automaticamente no navegador
- Exportar a cena como `.obj`, o projeto como `.json` ou uma imagem `.png`
- Layout adaptável a computador e celular (modelagem mais confortável no PC)

## 🕹️ Como usar

1. Abra o site ou `index.html`
2. Escolha uma forma no menu da esquerda, ou use um dos modelos prontos
3. Clique numa peça para selecioná-la
4. Selecione **Mover**, **Girar** ou **Escala** e arraste a peça
5. Ajuste cor, rotação e valores no painel direito
6. Clique em **Salvar** para baixar um projeto JSON

| Tecla / ação | Função |
| --- | --- |
| `G` | Mover |
| `R` | Girar |
| `S` | Escala |
| `F` | Focar objeto |
| `Delete` | Excluir objeto |
| `Ctrl + S` | Salvar projeto JSON |
| `Ctrl + Z` | Desfazer |
| `Ctrl + Y` | Refazer |
| Roda do mouse | Zoom |
| Arrastar fora do objeto | Girar câmera |
| `Shift` + arrastar o fundo | Mover câmera |

## 🚀 Publicar este repositório com GitHub Pages

Este repositório **já existe**. Não é necessário criar outro repositório nem enviar os arquivos novamente

1. Abra **Settings → Pages** neste repositório
2. Em **Build and deployment**, selecione **Deploy from a branch**
3. Selecione a branch `main` e a pasta `/(root)`
4. Clique em **Save**
5. Aguarde o GitHub Pages indicar que a publicação foi concluída e use o endereço mostrado nessa tela

A disponibilidade do endereço depende da configuração e da conclusão da publicação do GitHub Pages; a existência deste código no repositório, por si só, não comprova que o site esteja publicado

**Importante:** um site publicado pelo GitHub Pages pode ser visitado por outras pessoas. Se preferir manter o projeto só no seu computador, abra `index.html` offline e não ative o GitHub Pages

A página de suporte e seu catálogo também só ficarão disponíveis no site depois que as alterações correspondentes forem integradas e o GitHub Pages publicar os arquivos. Este pull request contém código e documentação, não é um novo Release nem comprova uma publicação do site

## 📁 Arquivos

```text
ChimpiBlender-Online/
├── .github/workflows/support-notice.yml
├── index.html
├── surpresa/index.html
├── support.html
├── support-notice.js
├── support-policy.json
├── SUPPORT.md
├── tests/
│   ├── support.test.cjs
│   └── verify_support_browser.py
├── README.md
├── LICENSE
└── .gitignore
```

---

Feito para o projeto **Chimpi-hackintosh** 💜

## 📜 Licença

Este repositório utiliza a **Apache License 2.0**, conforme o arquivo [LICENSE](LICENSE) já presente no projeto

## Aviso de suporte

Aviso traduzido, data de 04/11/2026 às 00h UTC, versões e limites de distribuição em [SUPPORT.md](SUPPORT.md)
