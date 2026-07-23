# Military Themes — VS Code Color Theme Extension

![VSCode](https://img.shields.io/badge/VS_Code-%23007ACC.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green.svg)
![Version](https://img.shields.io/badge/version-0.1.0-blue.svg)

Extensão de **Color Theme** para Visual Studio Code com estética **militar**, contendo 5 temas dark de alto contraste e legíveis.

## Temas inclusos

| Tema | Descrição |
|------|-----------|
| **Military Green Dark** | Verde escuro militar / Olive Drab |
| **Military Purple Ops** | Verde base + detalhes em roxo tático |
| **Military Gray Tactical** | Cinza militar (gun metal) + accents verdes |
| **Military Red Alert** | Verde escuro + vermelho military / blood red |
| **Military Blue Force** | Verde base + azul marinho tático / navy |

Todos os temas são **dark**, com melhorias de contraste e syntax highlighting completo:
- ✅ Cores mais vibrantes e alto contraste
- ✅ Syntax highlighting completo (keywords, funções, tipos, números, strings, comments)
- ✅ Estilos: bold, italic, underline em elementos específicos
- ✅ Mais de 80 tokens de cor por tema
- ✅ UI melhorada (borders, hover, seleção, peek view, merge editor)

---

## Como testar (F5)

1. Abra a pasta no VS Code
2. Pressione **F5**
3. Na nova janela, pressione **Ctrl+K Ctrl+T**
4. Escolha um tema Military

## Como empacotar (`.vsix`)

```bash
npm install -g @vscode/vsce
vsce package
code --install-extension *.vsix
```

## Como usar em qualquer PC

1. Gere o `.vsix` uma vez
2. Copie o `.vsix` para Pen drive / GitHub
3. Instale em cada PC com: `code --install-extension military-themes-0.1.0.vsix`
4. Ative o **VS Code Sync** (Configurações → Sincronização) para o tema ser lembrado automaticamente

---

## Estrutura do projeto

```
vscode-military-themes/
├── package.json
├── README.md
├── LICENSE
├── .vscodeignore
├── .gitignore
├── .vscode/
│   └── launch.json
├── themes/
│   ├── military-green-dark-color-theme.json
│   ├── military-purple-ops-color-theme.json
│   ├── military-gray-tactical-color-theme.json
│   ├── military-red-alert-color-theme.json
│   └── military-blue-force-color-theme.json
└── images/
    └── icon.png
```

---

## Contribuindo

1. Fork
2. `git checkout -b feature/nova-cor`
3. `git commit -m 'feat: adiciona nova paleta'`
4. `git push origin feature/nova-cor`
5. Abra um Pull Request

---

## Créditos

Desenvolvido por **Thales** com o auxílio de **Cline** 🤖

---

## License

MIT — Veja o arquivo [LICENSE](LICENSE) para mais detalhes.
