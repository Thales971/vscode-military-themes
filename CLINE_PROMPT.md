# PROMPT COMPLETO PARA O CLINE

Cole este texto inteiro no Cline e deixe ele executar passo a passo.

---

## Objetivo

Crie uma extensão completa de **Color Theme** para Visual Studio Code chamada **Military Themes** (publisher: Thales971).

A extensão deve conter **5 temas dark** com estética militar. Os temas devem ficar salvos permanentemente e aparecer no seletor oficial de Color Theme do VSCode (`Ctrl+K Ctrl+T`).

### Temas obrigatórios:

1. **Military Green Dark**  
   - Base: verde escuro militar / olive drab profundo  
   - Fundo principal: muito escuro (quase preto com tom verde)  
   - Accents: verde oliva e verde floresta  
   - Texto: off-white com leve tom verde

2. **Military Purple Ops**  
   - Mesma base verde escura  
   - Detalhes e highlights em roxo tático / purple militar  
   - Activity bar, badges e seleção com roxo

3. **Military Gray Tactical**  
   - Base cinza militar (gun metal / tactical gray)  
   - Accents em verde militar  
   - Visual mais "industrial" e limpo

4. **Military Red Alert**  
   - Base verde escura  
   - Accents e highlights em vermelho militar / blood red  
   - Status bar e badges em vermelho

5. **Military Blue Force**  
   - Base verde escura  
   - Accents em azul marinho tático / navy  
   - Visual mais "força aérea / navy"

---

## Estrutura de arquivos que você deve criar

```
vscode-military-themes/
├── package.json
├── README.md
├── LICENSE
├── .vscodeignore
├── .gitignore
├── themes/
│   ├── military-green-dark-color-theme.json
│   ├── military-purple-ops-color-theme.json
│   ├── military-gray-tactical-color-theme.json
│   ├── military-red-alert-color-theme.json
│   └── military-blue-force-color-theme.json
└── images/
    └── icon.png   (pode deixar placeholder por enquanto)
```

---

## package.json (obrigatório)

Crie um `package.json` completo e profissional com:

- name: `military-themes`
- displayName: `Military Themes`
- description: `Temas dark com estética militar: verde escuro, purple ops, gray tactical, red alert e blue force. Criado para programadores que gostam de vibe militar.`
- version: `0.1.0`
- publisher: `Thales971`
- engines.vscode: `^1.85.0`
- categories: `["Themes"]`
- keywords: `["theme", "military", "dark", "green", "olive", "tactical", "purple", "red", "blue"]`
- contributes.themes com os 5 temas (label, uiTheme: "vs-dark", path)
- repository, bugs, homepage apontando para https://github.com/Thales971/vscode-military-themes
- icon: `images/icon.png`

---

## Cores recomendadas (use como base e refine)

### Paleta base (Military Green Dark)

```json
{
  "editor.background": "#141a14",
  "editor.foreground": "#c8d0c0",
  "sideBar.background": "#1a2118",
  "activityBar.background": "#0f140f",
  "statusBar.background": "#2e3b2e",
  "titleBar.activeBackground": "#1a2118",
  "panel.background": "#1a2118",
  "terminal.background": "#141a14",
  "list.activeSelectionBackground": "#2e4a2e",
  "editor.selectionBackground": "#2e4a2e80",
  "editorLineNumber.foreground": "#5a6b5a",
  "editorLineNumber.activeForeground": "#a0b890",
  "focusBorder": "#4a6b4a",
  "button.background": "#3a5a3a",
  "button.hoverBackground": "#4a6b4a"
}
```

### Accents por tema

- **Purple Ops**: activityBarBadge, statusBar, focusBorder, list selection → `#6b4c7a` / `#8a6b9a`
- **Gray Tactical**: base cinza `#1e1e1e` / `#2a2a2a`, accents verde `#4a6b4a`
- **Red Alert**: accents `#8b2e2e` / `#a33a3a`
- **Blue Force**: accents `#2c4a6b` / `#3a5a7a`

Você deve preencher **muitos** tokens de cor (não só os básicos). Inclua pelo menos:

- editor.*
- sideBar.*
- activityBar.*
- statusBar.*
- titleBar.*
- panel.*
- terminal.*
- list.*
- tab.*
- input.*
- dropdown.*
- button.*
- badge.*
- scrollbarSlider.*
- gitDecoration.*
- editorSuggestWidget.*
- peekView.*
- etc.

Use a referência oficial: https://code.visualstudio.com/api/references/theme-color

Para `tokenColors` (syntax highlighting), crie regras boas para:
- comments (verde mais apagado)
- strings
- keywords
- functions
- types
- variables
- constants
- numbers
- etc.

Pode basear em um tema dark popular (ex: One Dark Pro ou Monokai) e adaptar as cores para a paleta militar.

---

## Passos que o Cline deve seguir (ordem)

1. Criar a estrutura de pastas e arquivos
2. Criar o `package.json` completo
3. Criar os 5 arquivos de tema em `themes/` com nome `-color-theme.json`
4. Preencher cada tema com `name`, `type: "dark"`, `colors` e `tokenColors` bem completos
5. Criar um README.md profissional (com preview dos temas, como instalar, como contribuir)
6. Criar `.vscodeignore` e `.gitignore`
7. Criar um LICENSE MIT simples
8. (Opcional) Criar um ícone simples ou deixar placeholder
9. No final, me mostrar como testar (F5) e como empacotar (`vsce package`)

---

## Requisitos de qualidade

- Temas devem ter **bom contraste** (legíveis)
- Não deixar cores "quebradas" (ex: texto preto em fundo preto)
- Manter consistência visual entre os 5 temas (só mudar accents)
- Comentários no código JSON onde fizer sentido
- Código limpo e organizado

---

## Depois de terminar

Mostre:
1. A árvore de arquivos final
2. Como testar localmente (F5)
3. Comando para gerar o `.vsix`
4. Como instalar o `.vsix` no VSCode

Pode começar agora. Execute o plano completo.
