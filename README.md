# Personal Agents Marketplace

[English](#personal-agents-marketplace) | [Português (Brasil)](#marketplace-de-agentes-pessoais)

A collection of specialized AI agents and professional skills designed for high-performance engineering teams and leadership development. This project is a **hybrid marketplace**, fully compatible with both **Claude Code** and **Gemini CLI**.

## 🚀 Plugins & Skills

### 1. Engineering Presentation Builder
*   **Domain**: Engineering & Technical Communication
*   **Goal**: Helps build structured, technical presentations, architecture overviews, and project deep-dives.
*   **Key Features**: Technical flow (Problem -> Solution -> Architecture), diagram standards, and framework-driven slides.

### 2. Lead Flow
*   **Domain**: Leadership & Strategic Communication
*   **Goal**: Strategic coaching for management, feedback cycles, team alignment, and professional communication.
*   **Key Features**: Diagnostic templates, difficult conversation preparation, and leadership alignment strategies.

---

## 🛠 Installation

### For Claude Code
This project uses the `marketplace.json` standard for Claude Code plugins. You can install it by pointing to this repository:

```bash
# Add the marketplace to Claude Code
claude plugins add https://github.com/rafaellemes/personal-agents

# Or install from a local directory during development
claude plugins add ./personal-agents
```

### For Gemini CLI
Each plugin is also a Gemini Skill (defined via `SKILL.md`).
To install the skills in your current workspace:

```bash
# Install Engineering Presentation Builder
gemini skills install ./plugins/engineering-presentation-builder --scope workspace

# Install Lead Flow
gemini skills install ./plugins/lead-flow --scope workspace

# Reload skills to activate
/skills reload
```

---

## 📁 Project Structure

```text
.
├── marketplace.json        # Central index for Claude Code
├── plugins/
│   ├── engineering-presentation-builder/
│   │   ├── .claude-plugin/ # Claude metadata
│   │   ├── SKILL.md        # Gemini metadata & instructions
│   │   ├── references/     # Shared knowledge base
│   │   └── assets/         # Shared templates/assets
│   └── lead-flow/
│       ├── .claude-plugin/
│       ├── SKILL.md
│       ├── references/
│       └── assets/
└── README.md
```

## 🤝 Contribution

This project follows a dual-compatibility standard. When adding new plugins:
1. Create the plugin structure under `plugins/`.
2. Include both `.claude-plugin/plugin.json` and `SKILL.md`.
3. Update `marketplace.json` in the root.
4. Keep shared logic (scripts, references) in their respective folders for reuse across both ecosystems.

## 📄 License
MIT

---

# Marketplace de Agentes Pessoais

[English](#personal-agents-marketplace) | [Português (Brasil)](#marketplace-de-agentes-pessoais)

Uma coleção de agentes de IA especializados e skills profissionais projetados para equipes de engenharia de alta performance e desenvolvimento de liderança. Este projeto é um **marketplace híbrido**, totalmente compatível com o **Claude Code** e o **Gemini CLI**.

## 🚀 Plugins & Skills

### 1. Engineering Presentation Builder
*   **Domínio**: Engenharia e Comunicação Técnica
*   **Objetivo**: Ajuda a construir apresentações técnicas estruturadas, visões gerais de arquitetura e mergulhos profundos em projetos.
*   **Recursos Principais**: Fluxo técnico (Problema -> Solução -> Arquitetura), padrões de diagramas e slides baseados em frameworks.

### 2. Lead Flow
*   **Domínio**: Liderança e Comunicação Estratégica
*   **Objetivo**: Coaching estratégico para gestão, ciclos de feedback, alinhamento de equipe e comunicação profissional.
*   **Recursos Principais**: Templates de diagnóstico, preparação para conversas difíceis e estratégias de alinhamento de liderança.

---

## 🛠 Instalação

### Para Claude Code
Este projeto utiliza o padrão `marketplace.json` para plugins do Claude Code. Você pode instalá-lo apontando para este repositório:

```bash
# Adicionar o marketplace ao Claude Code
claude plugins add https://github.com/rafaellemes/personal-agents

# Ou instalar a partir de um diretório local durante o desenvolvimento
claude plugins add ./personal-agents
```

### Para Gemini CLI
Cada plugin também é uma Gemini Skill (definida via `SKILL.md`).
Para instalar as skills no seu workspace atual:

```bash
# Instalar Engineering Presentation Builder
gemini skills install ./plugins/engineering-presentation-builder --scope workspace

# Instalar Lead Flow
gemini skills install ./plugins/lead-flow --scope workspace

# Recarregar as skills para ativar
/skills reload
```

---

## 🤝 Contribuição

Este projeto segue um padrão de compatibilidade dupla. Ao adicionar novos plugins:
1. Crie a estrutura do plugin em `plugins/`.
2. Inclua tanto o `.claude-plugin/plugin.json` quanto o `SKILL.md`.
3. Atualize o `marketplace.json` na raiz.
4. Mantenha a lógica compartilhada (scripts, referências) em suas respectivas pastas para reuso em ambos os ecossistemas.

## 📄 Licença
MIT
cossistemas.

## 📄 Licença
MIT
