---
name: ui-ux-pro-max-skill-main-skill-lovable
description: Use when the user wants to use, integrate, configure, or build with ui-ux-pro-max-skill-main — Skill gerada a partir do arquivo ui-ux-pro-max-skill-main.zip. Activate when the conversation mentions ui-ux-pro-max-skill-main.
---

# ui-ux-pro-max-skill-main

> Skill gerada a partir do arquivo ui-ux-pro-max-skill-main.zip.

**Repository:** https://github.com/local/ui-ux-pro-max-skill-main
**Language:** —  ·  **Stars:** 0  ·  **License:** —


## When to use this skill

Use when the user wants to use, integrate, configure, or build with ui-ux-pro-max-skill-main — Skill gerada a partir do arquivo ui-ux-pro-max-skill-main.zip. Activate when the conversation mentions ui-ux-pro-max-skill-main.

## Capabilities (from README)

- Recommended Pattern - Landing page structure
- Style Priority - Best matching UI styles
- Color Mood - Industry-appropriate palettes
- Typography Mood - Font personality matching
- Key Effects - Animations and interactions
- Anti-Patterns - What NOT to do (e.g., "AI purple/pink gradients" for banking)
- 67 UI Styles - Glassmorphism, Claymorphism, Minimalism, Brutalism, Neumorphism, Bento Grid, Dark Mode, AI-Native UI, and more
- 161 Color Palettes - Industry-specific palettes aligned 1:1 with the 161 product types

## Workflow

1. **Orient** — Confirm what the user wants to do with ui-ux-pro-max-skill-main.
2. **Recall** — Abra `REFERENCES.md` e localize a seção do doc relevante (mirror dos paths originais).
3. **Configure** — Walk through installation/setup; ask for missing env vars or credentials.
4. **Build** — Generate code/config that matches the conventions in the docs.
5. **Validate** — Run the project's own checks (tests, lints, smoke calls) before declaring done.
6. **Cite** — Quando responder, mencione qual seção de `REFERENCES.md` você usou.

## Conventions

- Prefer official APIs/CLI documented in the repo over third-party wrappers.
- Surface required env vars and secrets explicitly; never inline real values.
- If the repo ships a CLI, prefer its commands over re-implementing logic.

## Sanitização de Dados (DLP — obrigatório)

Esta skill opera sob política **Zero Trust**. Antes de qualquer resposta, log ou
artefato gerado:

- **Nunca** exponha em logs, UI pública ou commits: chaves de API, tokens, senhas,
  strings de conexão, JWTs, dados de PII (CPF, CNPJ, e-mail real, telefone) ou
  conteúdo de arquivos `.env` reais.
- Ao citar valores sensíveis, substitua por placeholder: `ENV_VAR_PLACEHOLDER`,
  `*****` ou `<REDACTED>`.
- Toda credencial deve ser lida via `process.env.NOME_DA_VAR` — nunca hard-coded.
- Arquivos de configuração entregues ao usuário devem ser **templates** sem valores
  reais (ex.: `.env.example` com `API_KEY=ENV_VAR_PLACEHOLDER`).
- Antes de enviar dados do usuário a APIs terceiras, valide o destino e mascare
  PII que não seja estritamente necessária à chamada.

## Mitigar Riscos de Dados (mecanismo de ação)

Quando o usuário pedir **"mitigar riscos"**, **"sanitizar"** ou for solicitar
deploy/publicação, execute este protocolo antes de qualquer outra coisa:

1. **Validar** — varra o contexto atual e os arquivos gerados procurando:
   `sk_live_*`, `sk_test_*`, `pk_live_*`, `whsec_*`, `AIzaSy*`, `ghp_*`,
   `AKIA*`, `xox[baprs]-*`, `SG.*`, JWTs (`eyJ...`), connection strings
   (`postgres://user:pass@...`), CPF/CNPJ, e arquivos `.env` com valores reais.
2. **Interromper** — se algum padrão for encontrado, **pare o fluxo** e reporte
   o achado ao usuário antes de prosseguir. Não gere, não envie, não comite.
3. **Mascarar** — substitua o valor sensível por `ENV_VAR_PLACEHOLDER` (ou
   `*****` para PII) tanto no código quanto em logs/respostas.
4. **Corrigir o código** — converta chamadas inseguras (`fetch("https://api/?key=ABC123")`,
   credenciais inline em headers/SDK) para usar `process.env.X` e instrua o
   usuário a configurar a variável no ambiente.
5. **Substituir `.env` por `.env.example`** — se um `.env` real for detectado,
   gere um `.env.example` com placeholders e remova o arquivo original.
6. **Reportar** — ao final, devolva um sumário: o que foi mascarado, o que foi
   substituído, e quais ações o usuário ainda precisa executar (rotacionar
   chaves vazadas, configurar variáveis de ambiente, revisar diffs).

Se algum risco crítico não puder ser mitigado automaticamente, **recomende não
publicar** o artefato e oriente revisão manual.

## Reference index (consolidado em REFERENCES.md)

- `README.md` (consultar seção em `REFERENCES.md`)
- `cli/README.md` (consultar seção em `REFERENCES.md`)
- `CLAUDE.md` (consultar seção em `REFERENCES.md`)
- `CONTRIBUTING.md` (consultar seção em `REFERENCES.md`)
- `docs/三个 data-scripts-templates 的区别.md` (consultar seção em `REFERENCES.md`)
- `.claude/skills/banner-design/SKILL.md` (consultar seção em `REFERENCES.md`)
- `.claude/skills/brand/SKILL.md` (consultar seção em `REFERENCES.md`)
- `.claude/skills/design-system/SKILL.md` (consultar seção em `REFERENCES.md`)
- `.claude/skills/design/SKILL.md` (consultar seção em `REFERENCES.md`)
- `.claude/skills/slides/SKILL.md` (consultar seção em `REFERENCES.md`)
- `.claude/skills/ui-styling/SKILL.md` (consultar seção em `REFERENCES.md`)
- `.claude/skills/ui-ux-pro-max/SKILL.md` (consultar seção em `REFERENCES.md`)
- `.claude/skills/banner-design/references/banner-sizes-and-styles.md` (consultar seção em `REFERENCES.md`)
- `.claude/skills/brand/references/approval-checklist.md` (consultar seção em `REFERENCES.md`)
- `.claude/skills/brand/references/asset-organization.md` (consultar seção em `REFERENCES.md`)
- `.claude/skills/brand/references/brand-guideline-template.md` (consultar seção em `REFERENCES.md`)
- `.claude/skills/brand/references/color-palette-management.md` (consultar seção em `REFERENCES.md`)
- `.claude/skills/brand/references/consistency-checklist.md` (consultar seção em `REFERENCES.md`)
- `.claude/skills/brand/references/logo-usage-rules.md` (consultar seção em `REFERENCES.md`)
- `.claude/skills/brand/references/messaging-framework.md` (consultar seção em `REFERENCES.md`)
- `.claude/skills/brand/references/typography-specifications.md` (consultar seção em `REFERENCES.md`)
- `.claude/skills/brand/references/update.md` (consultar seção em `REFERENCES.md`)
- `.claude/skills/brand/references/visual-identity.md` (consultar seção em `REFERENCES.md`)
- `.claude/skills/brand/references/voice-framework.md` (consultar seção em `REFERENCES.md`)
- `.claude/skills/brand/templates/brand-guidelines-starter.md` (consultar seção em `REFERENCES.md`)
- `_metadata.json` — Repo metadata snapshot.


## Complete repository map

```
  - marketplace.json
  - plugin.json
        - banner-sizes-and-styles.md
      - SKILL.md
        - approval-checklist.md
        - asset-organization.md
        - brand-guideline-template.md
        - color-palette-management.md
        - consistency-checklist.md
        - logo-usage-rules.md
        - messaging-framework.md
        - typography-specifications.md
        - update.md
        - visual-identity.md
        - voice-framework.md
        - extract-colors.cjs
        - inject-brand-context.cjs
        - sync-brand-to-tokens.cjs
        - validate-asset.cjs
      - SKILL.md
        - brand-guidelines-starter.md
        - slide-backgrounds.csv
        - slide-charts.csv
        - slide-color-logic.csv
        - slide-copy.csv
        - slide-layout-logic.csv
        - slide-layouts.csv
        - slide-strategies.csv
        - slide-typography.csv
        - component-specs.md
        - component-tokens.md
        - primitive-tokens.md
        - semantic-tokens.md
        - states-and-variants.md
        - tailwind-integration.md
        - token-architecture.md
        - embed-tokens.cjs
        - fetch-background.py
        - generate-slide.py
        - generate-tokens.cjs
        - html-token-validator.py
        - search-slides.py
        - slide_search_core.py
        - slide-token-validator.py
        - validate-tokens.cjs
      - SKILL.md
        - design-tokens-starter.json
          - deliverables.csv
          - industries.csv
          - mockup-contexts.csv
          - styles.csv
          - styles.csv
          - colors.csv
          - industries.csv
          - styles.csv
        - banner-sizes-and-styles.md
        - cip-deliverable-guide.md
        - cip-design.md
        - cip-prompt-engineering.md
        - cip-style-guide.md
        - design-routing.md
        - icon-design.md
        - logo-color-psychology.md
        - logo-design.md
        - logo-prompt-engineering.md
        - logo-style-guide.md
        - slides-copywriting-formulas.md
        - slides-create.md
        - slides-html-template.md
        - slides-layout-patterns.md
        - slides-strategies.md
        - slides.md
        - social-photos-design.md
          - core.py
          - generate.py
          - render-html.py
          - search.py
          - generate.py
          - core.py
          - generate.py
          - search.py
      - SKILL.md
        - copywriting-formulas.md
        - create.md
        - html-template.md
        - layout-patterns.md
        - slide-strategies.md
      - SKILL.md
        - ArsenalSC-OFL.txt
        - ArsenalSC-Regular.ttf
        - BigShoulders-Bold.ttf
        - BigShoulders-OFL.txt
        - BigShoulders-Regular.ttf
        - Boldonse-OFL.txt
        - Boldonse-Regular.ttf
        - BricolageGrotesque-Bold.ttf
        - BricolageGrotesque-OFL.txt
        - BricolageGrotesque-Regular.ttf
        - CrimsonPro-Bold.ttf
        - CrimsonPro-Italic.ttf
        - CrimsonPro-OFL.txt
        - CrimsonPro-Regular.ttf
        - DMMono-OFL.txt
        - DMMono-Regular.ttf
        - EricaOne-OFL.txt
        - EricaOne-Regular.ttf
        - GeistMono-Bold.ttf
        - GeistMono-OFL.txt
        - GeistMono-Regular.ttf
        - Gloock-OFL.txt
        - Gloock-Regular.ttf
        - IBMPlexMono-Bold.ttf
        - IBMPlexMono-OFL.txt
        - IBMPlexMono-Regular.ttf
        - IBMPlexSerif-Bold.ttf
        - IBMPlexSerif-BoldItalic.ttf
        - IBMPlexSerif-Italic.ttf
        - IBMPlexSerif-Regular.ttf
        - InstrumentSans-Bold.ttf
        - InstrumentSans-BoldItalic.ttf
        - InstrumentSans-Italic.ttf
        - InstrumentSans-OFL.txt
        - InstrumentSans-Regular.ttf
        - InstrumentSerif-Italic.ttf
        - InstrumentSerif-Regular.ttf
        - Italiana-OFL.txt
        - Italiana-Regular.ttf
        - JetBrainsMono-Bold.ttf
        - JetBrainsMono-OFL.txt
        - JetBrainsMono-Regular.ttf
        - Jura-Light.ttf
        - Jura-Medium.ttf
        - Jura-OFL.txt
        - LibreBaskerville-OFL.txt
        - LibreBaskerville-Regular.ttf
        - Lora-Bold.ttf
        - Lora-BoldItalic.ttf
        - Lora-Italic.ttf
        - Lora-OFL.txt
        - Lora-Regular.ttf
        - NationalPark-Bold.ttf
        - NationalPark-OFL.txt
        - NationalPark-Regular.ttf
        - NothingYouCouldDo-OFL.txt
        - NothingYouCouldDo-Regular.ttf
        - Outfit-Bold.ttf
        - Outfit-OFL.txt
        - Outfit-Regular.ttf
        - PixelifySans-Medium.ttf
        - PixelifySans-OFL.txt
        - PoiretOne-OFL.txt
        - PoiretOne-Regular.ttf
        - RedHatMono-Bold.ttf
        - RedHatMono-OFL.txt
        - RedHatMono-Regular.ttf
        - Silkscreen-OFL.txt
        - Silkscreen-Regular.ttf
        - SmoochSans-Medium.ttf
        - SmoochSans-OFL.txt
        - Tektur-Medium.ttf
        - Tektur-OFL.txt
        - Tektur-Regular.ttf
        - WorkSans-Bold.ttf
        - WorkSans-BoldItalic.ttf
        - WorkSans-Italic.ttf
        - WorkSans-OFL.txt
        - WorkSans-Regular.ttf
        - YoungSerif-OFL.txt
        - YoungSerif-Regular.ttf
      - LICENSE.txt
        - canvas-design-system.md
        - shadcn-accessibility.md
        - shadcn-components.md
        - shadcn-theming.md
        - tailwind-customization.md
        - tailwind-responsive.md
        - tailwind-utilities.md
        - .coverage
        - requirements.txt
        - shadcn_add.py
        - tailwind_config_gen.py
          - coverage-ui.json
          - requirements.txt
          - test_shadcn_add.py
          - test_tailwind_config_gen.py
      - SKILL.md
      - data
      - scripts
      - SKILL.md
    - release.yml
- .gitignore
- .releaserc.json
- CLAUDE.md
  - .gitignore
  - .npmignore
      - _sync_all.py
      - app-interface.csv
      - charts.csv
      - colors.csv
      - design.csv
      - draft.csv
      - google-fonts.csv
      - icons.csv
      - landing.csv
      - products.csv
      - react-performance.csv
        - angular.csv
        - astro.csv
        - flutter.csv
        - html-tailwind.csv
        - javafx.csv
        - jetpack-compose.csv
        - laravel.csv
        - nextjs.csv
        - nuxt-ui.csv
        - nuxtjs.csv
        - react-native.csv
        - react.csv
        - shadcn.csv
        - svelte.csv
        - swiftui.csv
        - threejs.csv
        - vue.csv
      - styles.csv
      - typography.csv
      - ui-reasoning.csv
      - ux-guidelines.csv
      - core.py
      - design_system.py
      - search.py
        - quick-reference.md
        - skill-content.md
        - agent.json
        - augment.json
        - claude.json
        - codebuddy.json
        - codex.json
        - continue.json
        - copilot.json
        - cursor.json
        - droid.json
        - gemini.json
        - kilocode.json
        - kiro.json
        - opencode.json
        - qoder.json
        - roocode.json
        - trae.json
        - warp.json
        - windsurf.json
  - bun.lock
  - package-lock.json
  - package.json
  - README.md
      - init.ts
      - uninstall.ts
      - update.ts
      - versions.ts
    - index.ts
      - index.ts
      - detect.ts
      - extract.ts
      - github.ts
      - logger.ts
      - template.ts
  - tsconfig.json
- CONTRIBUTING.md
  - 三个 data-scripts-templates 的区别.md
- LICENSE
  - xiaomaomi-app.html
- README.md
  - website.png
  - sync-release-version.mjs
- skill.json
      - _sync_all.py
      - app-interface.csv
      - charts.csv
      - colors.csv
      - design.csv
      - draft.csv
      - google-fonts.csv
      - icons.csv
      - landing.csv
      - products.csv
      - react-performance.csv
        - angular.csv
        - astro.csv
        - flutter.csv
        - html-tailwind.csv
        - javafx.csv
        - jetpack-compose.csv
        - laravel.csv
        - nextjs.csv
        - nuxt-ui.csv
        - nuxtjs.csv
        - react-native.csv
        - react.csv
        - shadcn.csv
        - svelte.csv
        - swiftui.csv
        - threejs.csv
        - vue.csv
      - styles.csv
      - typography.csv
      - ui-reasoning.csv
      - ux-guidelines.csv
      - core.py
      - design_system.py
      - search.py
        - quick-reference.md
        - skill-content.md
        - agent.json
        - augment.json
        - claude.json
        - codebuddy.json
        - codex.json
        - continue.json
        - copilot.json
        - cursor.json
        - droid.json
        - gemini.json
        - kilocode.json
        - kiro.json
        - opencode.json
        - qoder.json
        - roocode.json
        - trae.json
        - warp.json
        - windsurf.json
```
