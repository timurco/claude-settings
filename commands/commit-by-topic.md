Make commits using structured approach:

#### **Commit Structure:**
- **Format:** Use heredoc for multiline commit messages to ensure proper line breaks
- **Language:** All commit messages MUST be in English
- **Types with emojis:**
  - `✨ feat:` - New features
  - `🐛 fix:` - Bug fixes
  - `📚 docs:` - Documentation changes
  - `🎨 style:` - Code style/formatting
  - `♻️ refactor:` - Code refactoring
  - `🧪 test:` - Tests
  - `🔧 chore:` - Maintenance tasks
  - `🏗️ build:` - Build system changes
  - `⚙️ ci:` - CI/CD changes

#### **Commit Process:**
1. **Analyze:** Review `git status` and `git diff`
2. **Group by topic:** Group as many related files as possible into single commits by topic.
3. **Stage:** `git add` all files belonging to the same topic/feature
4. **Commit:** Use heredoc format for multiline messages

#### **Examples:**
```bash
git commit -m "
✨ feat: add MapConverter for URL conversion

- Add Node.js project structure
- Implement clipboard support for macOS"

git commit -m "
🐛 fix: correct gitignore corrupted entries

- Fix first line corruption
- Add Node.js patterns
- Remove duplicates"

git commit -m "
📚 docs: update repository guidelines

- Add development guidelines for LLM
- Include commit message standards"
```

**Rule:** Maximize files per commit by topic. Only split commits when dealing with completely unrelated changes.
**Format:** Always use heredoc format with ` ... EOF)` to ensure proper line breaks in commit messages.