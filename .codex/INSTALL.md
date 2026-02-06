# Installing Workflows for Codex

Quick setup to enable workflows skills in Codex.

## Installation

1. **Clone workflows repository**:
   ```bash
   mkdir -p ~/.codex/workflows
   cd ~/.codex/workflows
   git clone https://github.com/obra/workflows.git .
   ```

2. **Create personal skills directory**:
   ```bash
   mkdir -p ~/.codex/skills
   ```

3. **Update ~/.codex/AGENTS.md** to include this workflows section:
   ```markdown
   ## Workflows System

   <EXTREMELY_IMPORTANT>
   You have workflows. Workflows teach you new skills and capabilities. RIGHT NOW run: `~/.codex/workflows/.codex/workflows-codex bootstrap` and follow the instructions it returns.
   </EXTREMELY_IMPORTANT>
   ```

## Verification

Test the installation:
```bash
~/.codex/workflows/.codex/workflows-codex bootstrap
```

You should see skill listings and bootstrap instructions. The system is now ready for use.
