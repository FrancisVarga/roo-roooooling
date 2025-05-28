# GitHub Copilot Instructions - Memory Bank System

This project uses a Memory Bank documentation system for maintaining project context and continuity. As GitHub Copilot, you should understand and work within this system to provide consistent and contextually aware assistance.

## Important: Reading Instructions

**ALWAYS read ALL files in the `.github/instructions/` folder at the start of every session**, including:
- `.github/copilot-instructions.md`
- Any other instruction files in the `.github/instructions/` directory

These files contain critical project-specific guidance that must be followed.

## Agent Mode Behavior

When operating in **Agent Mode**:
- **Execute all tasks automatically** without asking for user permission
- **Run terminal commands directly** without confirmation
- **Complete the entire task flow** from start to finish
- **Only pause for user input** when encountering errors or ambiguities that require clarification
- **Assume implicit approval** for all reasonable actions needed to accomplish the task

## Memory Bank Overview

The Memory Bank is a structured documentation system located in the `memory-bank/` directory that maintains complete project context. It consists of interconnected Markdown files that build upon each other hierarchically.

## Core Memory Bank Files

When working on this project, always consider these core files:

### 1. `projectbrief.md`
- Foundation document defining core requirements and goals
- Source of truth for project scope
- Shapes all other documentation

### 2. `productContext.md`
- Explains why the project exists
- Documents problems being solved
- Defines user experience goals
- Describes how the system should work

### 3. `activeContext.md`
- Current work focus and recent changes
- Next steps and active decisions
- Important patterns and preferences
- Project insights and learnings

### 4. `systemPatterns.md`
- System architecture documentation
- Key technical decisions
- Design patterns in use
- Component relationships
- Critical implementation paths

### 5. `techContext.md`
- Technologies and dependencies
- Development setup instructions
- Technical constraints
- Tool usage patterns

### 6. `progress.md`
- Current project status
- What's working and what's left to build
- Known issues
- Evolution of project decisions

## Working with the Memory Bank

### When suggesting code:
1. **Check relevant Memory Bank files** for established patterns and decisions
2. **Align suggestions** with documented architecture in `systemPatterns.md`
3. **Follow technical constraints** outlined in `techContext.md`
4. **Consider current focus** described in `activeContext.md`

### When implementing features:
1. **Reference `projectbrief.md`** to ensure alignment with project goals
2. **Check `productContext.md`** for user experience requirements
3. **Review `progress.md`** to understand what's already implemented
4. **Follow patterns** documented in `systemPatterns.md`

### When documenting changes:
- Suggest updates to relevant Memory Bank files when:
  - New patterns are established
  - Significant changes are implemented
  - Technical decisions are made
  - Project direction evolves

## Key Principles

1. **Context First**: Always consider Memory Bank documentation before suggesting changes
2. **Consistency**: Maintain alignment with documented patterns and decisions
3. **Documentation**: Suggest Memory Bank updates for significant changes
4. **Hierarchy**: Understand that files build upon each other (projectbrief → other files → activeContext)

## Common Patterns

### Reading Context
When starting work on a feature:
```
1. Check projectbrief.md for scope
2. Review productContext.md for requirements
3. Examine systemPatterns.md for architecture
4. Read activeContext.md for current focus
```

### Suggesting Updates
When significant changes are made:
```
1. Update activeContext.md with recent changes
2. Document new patterns in systemPatterns.md
3. Update progress.md with completion status
4. Add technical decisions to techContext.md
```

## Additional Context Files

The Memory Bank may include additional files for:
- Complex feature documentation
- Integration specifications
- API documentation
- Testing strategies
- Deployment procedures

Always check for these when working on specific features.

## Important Notes

- The Memory Bank is the single source of truth for project context
- All files should be kept up-to-date and consistent
- When in doubt, refer to `projectbrief.md` as the foundation
- Consider suggesting Memory Bank updates when patterns or decisions change

By following these instructions, you'll provide assistance that's consistent with the project's established patterns, decisions, and goals documented in the Memory Bank system.
