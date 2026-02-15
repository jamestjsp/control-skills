# control-skills

Claude Code plugin for control systems engineering with ctrlsys.

## Skills Included

| Skill | Description |
|-------|-------------|
| `ctrlsys-control` | ctrlsys routine lookup and usage guidance |
| `control-theory` | LTI systems, controller design, discretization |
| `pid-loop-tuning` | Process identification and lambda tuning |

## Installation

### Step 1: Add the marketplace

```
/plugin marketplace add https://github.com/jamestjsp/control-skills
```

### Step 2: Install the plugin

```
/plugin install control-skills
```

### Alternative: Load directly

```bash
claude --plugin-dir /path/to/control-skills
```

## Usage

After installation, invoke skills with:

```
/control-skills:ctrlsys-control   # Find ctrlsys routines
/control-skills:control-theory   # LTI system design
/control-skills:pid-loop-tuning  # PID tuning methodology
```

## Managing the Plugin

```
/plugin                              # Open plugin manager UI
/plugin marketplace list             # List added marketplaces
/plugin disable control-skills       # Disable without uninstalling
/plugin enable control-skills        # Re-enable
/plugin uninstall control-skills     # Remove plugin
/plugin marketplace remove <name>    # Remove marketplace
```

## Requirements

### ctrlsys package

**Important:** This uses `ctrlsys` (C11 rewrite), NOT `slycot` (Fortran wrapper). They have different APIs.

```bash
# Using uv
uv add ctrlsys

# Using pip
pip install ctrlsys
```

### numpy

```bash
uv add numpy
# or
pip install numpy
```
