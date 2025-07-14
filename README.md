# Personal Documentation Manager

A powerful command-line tool for managing your personal shell script documentation. Quickly create, edit, search, and organize your command references and documentation files.

## Installation

### Method 1: Quick Install (Recommended)

```bash
git clone <repository-url>
cd Personal-Doc
./doc --install
```

The `--install` command will:

- Create necessary directories
- Add the script to your shell's PATH
- Work with zsh, bash, or fish shells

### Method 2: Manual Install

```bash
# Clone and add to your personal bin
git clone <repository-url>
cd Personal-Doc
cp doc ~/bin/  # or any directory in your PATH
```

After installation, restart your terminal or run `source ~/.zshrc` (or your shell's config file).

## Usage

### Basic Commands

| Command | Description |
|---------|-------------|
| `doc` | List all documentation files |
| `doc -l` | List files with details (size, date) |
| `doc filename` | View contents of a specific file |
| `doc -e filename` | Edit or create a new file |
| `doc -s "query"` | Search files for content |
| `doc -x filename` | Archive a file |
| `doc -r filename` | Remove a file (with confirmation) |
| `doc -r filename -f` | Force remove without confirmation |

### Examples

```bash
# List all documentation files
doc

# List with file details
doc -l

# View a specific file
doc ssh-commands

# Edit or create a new file
doc -e docker-tips

# Search for files containing "git"
doc -s "git"

# Archive an old file
doc -x old-commands

# Remove a file (will ask for confirmation)
doc -r unused-file

# Force remove without confirmation
doc -r temp-file -f

# Install the tool system-wide
doc --install
```

#### File Organization

- All files are stored in `docs/` directory
- Archived files go to `docs/archived/`
- Files automatically get `.sh` extension
- Duplicate archive names are handled automatically
