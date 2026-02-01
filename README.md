# control-skills

Claude Code plugin for control systems engineering.

## Skills Included

| Skill | Description |
|-------|-------------|
| `/slicot-control` | SLICOT routine lookup and usage guidance |
| `/control-theory` | LTI systems, controller design, discretization |
| `/pid-loop-tuning` | Process identification and lambda tuning |

## Installation

```bash
/plugin marketplace add https://github.com/josephj/control-skills
/plugin install control-skills
```

Or load directly:

```bash
claude --plugin-dir /path/to/control-skills
```

## Requirements

- `slicot` package (C11 rewrite, NOT slycot)
- numpy

## Usage

Invoke skills with `/control-skills:<skill-name>`:

```
/control-skills:slicot-control   # Find SLICOT routines
/control-skills:control-theory   # LTI system design
/control-skills:pid-loop-tuning  # PID tuning methodology
```
