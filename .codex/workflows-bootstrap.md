# Workflows Bootstrap for Codex

<EXTREMELY_IMPORTANT>
You have workflows.

**Tool for running skills:**
- `~/.codex/workflows/.codex/workflows-codex use-skill <skill-name>`

**Tool Mapping for Codex:**
When skills reference tools you don't have, substitute your equivalent tools:
- `TodoWrite` → `update_plan` (your planning/task tracking tool)
- `Task` tool with subagents → Use Codex collab `spawn_agent` + `wait` when available; if collab is disabled, state that and proceed sequentially
- `Subagent` / `Agent` tool mentions → Map to `spawn_agent` (collab) or sequential fallback when collab is disabled
- `Skill` tool → `~/.codex/workflows/.codex/workflows-codex use-skill` command (already available)
- `Read`, `Write`, `Edit`, `Bash` → Use your native tools with similar functions

**Skills naming:**
- Workflows skills: `workflows:skill-name` (from ~/.codex/workflows/skills/)
- Personal skills: `skill-name` (from ~/.codex/skills/)
- Personal skills override workflows skills when names match

**Critical Rules:**
- Before ANY task, review the skills list (shown below)
- If a relevant skill exists, you MUST use `~/.codex/workflows/.codex/workflows-codex use-skill` to load it
- Announce: "I've read the [Skill Name] skill and I'm using it to [purpose]"
- Skills with checklists require `update_plan` todos for each item
- NEVER skip mandatory workflows (brainstorming before coding, TDD, systematic debugging)

**Skills location:**
- Workflows skills: ~/.codex/workflows/skills/
- Personal skills: ~/.codex/skills/ (override workflows when names match)

IF A SKILL APPLIES TO YOUR TASK, YOU DO NOT HAVE A CHOICE. YOU MUST USE IT.
</EXTREMELY_IMPORTANT>
