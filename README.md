# 🐒 ChimpiBlender Online

**Seu mini estúdio 3D no navegador, em português e sem instalação** 💜

![Prévia do ChimpiBlender Online](preview.png)

O ChimpiBlender Online é um editor 3D leve, desenvolvido em **HTML, CSS e JavaScript puro**. Ele funciona sem bibliotecas externas e também pode ser aberto offline. O modelo inicial é o **GatinhoMamãe**, com uma segunda cena conceitual de suporte para **tag NFC**.

> **Observação:** este é um editor 3D independente, **não é o Blender oficial**. Ele não gera instruções para caneta 3D nem grava tags NFC.

## 🌐 Acessar o editor

Depois de ativar o GitHub Pages, o site ficará disponível em:

`https://chimpi-hackintosh.github.io/ChimpiBlender-Online/`

**Antes da publicação:** abra `index.html` diretamente no navegador do computador, ou use um servidor local para testar.

## ✨ Funcionalidades

- Modelos 3D: cubo, esfera, cilindro, cone, rosca e plano
- Mover, girar, redimensionar, duplicar, excluir e colorir objetos
- Câmera orbital com zoom, panorâmica e foco
- Cena do **GatinhoMamãe** e exemplo visual para a base de uma tag NFC
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

## 🚀 Publicar com GitHub Pages (sem terminal)

1. Crie um repositório **público** chamado `ChimpiBlender-Online` em sua conta GitHub
2. Dentro dele, clique em **Add file → Upload files**
3. Envie os **arquivos extraídos da pasta**, especialmente `index.html` na raiz, sem uma pasta extra
4. Clique em **Commit changes**
5. Abra **Settings → Pages**
6. Em **Build and deployment**, selecione **Deploy from a branch**
7. Selecione `main`, pasta `/(root)` e clique em **Save**
8. Aguarde o GitHub concluir a publicação e abra o endereço indicado no topo deste README

**Importante:** um site publicado pelo GitHub Pages pode ser visitado por outras pessoas. Se preferir manter o projeto só no seu computador, basta abrir `index.html` offline e não ativar o GitHub Pages.

## 📁 Arquivos

```
ChimpiBlender-Online/
├── index.html       # Editor 3D completo
├── preview.png      # Prévia real do aplicativo
├── README.md        # Documentação
├── LICENSE          # Licença MIT
└── .gitignore       # Arquivos ignorados pelo Git
```

## 🐱 GatinhoMamãe e caneta 3D

O modelo de suporte NFC é **apenas uma referência de formato**. Meça a tag real antes de projetar o suporte físico. **Não aqueça uma tag NFC com a caneta 3D**, pois o calor pode danificá-la. Construa e deixe a peça esfriar antes de colocar a tag.

---

Feito para o projeto **Chimpi-hackintosh** 💜