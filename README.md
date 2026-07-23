# VSCode Military Themes

Extensão personalizada de temas para VSCode com estética **militar**, criada especialmente para o Thales.

## Temas inclusos (objetivo final)

1. **Military Green Dark** — Verde escuro militar (olive drab / forest dark)
2. **Military Purple Ops** — Verde base + detalhes em roxo tático
3. **Military Gray Tactical** — Cinza militar + accents verdes
4. **Military Red Alert** — Verde escuro + vermelho militar (alerta)
5. **Military Blue Force** — Verde + azul marinho tático

Todos são **dark themes**, com contraste alto, legíveis por longas sessões de código, e ficam salvos permanentemente nas configurações de extensão do VSCode (aparecem no seletor oficial de Color Theme).

## Como gerar a extensão com o Cline

1. Clone este repositório:
   ```bash
   git clone https://github.com/Thales971/vscode-military-themes.git
   cd vscode-military-themes
   ```

2. Abra a pasta no VSCode

3. Abra o **Cline** e cole o conteúdo completo do arquivo **`CLINE_PROMPT.md`**

4. Deixe o Cline executar o plano passo a passo (ele vai criar package.json, pastas themes/, os 5 arquivos de tema, README final, etc.)

5. Depois de pronto, teste com **F5** (abre Extension Development Host)

6. Para instalar localmente:
   ```bash
   npm install -g @vscode/vsce
   vsce package
   code --install-extension *.vsix
   ```

## Status do projeto

- [x] Repositório criado
- [x] Prompt detalhado para o Cline (`CLINE_PROMPT.md`)
- [ ] Scaffold completo da extensão
- [ ] 5 temas coloridos definidos
- [ ] package.json + contributes.themes
- [ ] README final + screenshots
- [ ] Publicação no Marketplace (opcional)

---

Feito com vibe code 🚀  
Thales Vitor Boehm + Grok + Cline
