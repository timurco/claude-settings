# Claude Settings Repository

This is my personal repository ([@timurco/claude-settings](https://github.com/timurco/claude-settings.git)) where I store my Claude AI assistant settings, commands, and other configuration files.

### Setup

Go to User/.cluade

```bash
git init

git remote add origin https://github.com/timurco/claude-settings.git

# Fetch latest changes from remote
git fetch origin

# Force reset local branch to match remote branch
git reset --hard origin/main
```

**Warning**: This will permanently delete any uncommitted local changes. Make sure to backup important work before running these commands.

## What's Inside

Currently, this repository contains primarily **commands** - custom instructions and workflows I use with Claude. The repository is structured to keep everything organized and easily accessible.

## Commands

### 📝 Commit Commands

I maintain two different approaches for Git commits, depending on the complexity of the changes:

#### `commit-all.md`
A straightforward commit approach for simple, single-topic changes:
- Uses structured commit messages with emojis
- Supports multiline messages with heredoc format
- All messages must be in English
- Covers common commit types: features, fixes, docs, style, refactor, tests, chores, build, and CI changes

#### `commit-by-topic.md`
An advanced commit strategy for complex changes:
- Groups related files by topic into single commits
- Maximizes files per commit to maintain logical grouping
- Uses heredoc format (`$(cat <<'EOF' ... EOF)`) for proper multiline message formatting
- Includes a step-by-step process: analyze → group → stage → commit
- Rule: Only split commits for completely unrelated changes

Both commands follow consistent emoji-based commit type conventions:
- ✨ `feat:` - New features
- 🐛 `fix:` - Bug fixes
- 📚 `docs:` - Documentation changes
- 🎨 `style:` - Code style/formatting
- ♻️ `refactor:` - Code refactoring
- 🧪 `test:` - Tests
- 🔧 `chore:` - Maintenance tasks
- 🏗️ `build:` - Build system changes
- ⚙️ `ci:` - CI/CD changes

## Usage

Feel free to explore and adapt any of these commands for your own workflow. All content is organized for easy reference and modification.

## License

This repository is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
