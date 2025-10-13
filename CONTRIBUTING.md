# Contributing to Hermetic Agents Pack

Thank you for your interest in contributing! This document provides guidelines and instructions for contributing to the Hermetic Agents Pack.

---

## 🎯 Ways to Contribute

### 1. Report Bugs
Found a bug? Help us improve!

**Before submitting:**
- Check if the issue already exists
- Use the latest version
- Gather reproduction steps

**Submit via:**
- [GitHub Issues](https://github.com/ormus/hermetic-agents-pack/issues)

**Include:**
- Clear description of the problem
- Steps to reproduce
- Expected vs actual behavior
- Claude Code version
- Operating system
- Screenshots/logs if applicable

### 2. Suggest New Agents
Have an idea for a new specialized agent?

**Good agent suggestions include:**
- Clear domain/specialization
- Specific use cases (at least 3)
- Why it's needed (gap it fills)
- How it differs from existing agents

**Submit via:**
- [GitHub Discussions](https://github.com/ormus/hermetic-agents-pack/discussions)

### 3. Improve Existing Agents
Help make agents better!

**Areas for improvement:**
- Agent descriptions clarity
- Usage examples
- Tool restrictions
- Response quality
- Edge case handling

**Submit via:**
- Pull request with specific improvements
- Issue describing the improvement

### 4. Write Documentation
Documentation is always appreciated!

**Help needed:**
- Usage examples
- Tutorials
- Best practices guides
- Troubleshooting tips
- Translation to other languages

### 5. Share Usage Stories
Inspire others with your success!

**Share:**
- What you built with the agents
- Time saved
- Productivity improvements
- Favorite agents and workflows
- Tips and tricks

**Submit via:**
- GitHub Discussions
- Blog posts (we'll link to them!)
- Social media (tag us!)

---

## 📝 Pull Request Guidelines

### Before You Start
1. **Check existing PRs** - Someone might be working on it
2. **Open an issue first** - Discuss major changes
3. **One change per PR** - Keep PRs focused

### Making Changes

**For Agent Improvements:**
1. Keep agent structure consistent
2. Maintain markdown format
3. Include clear examples
4. Test with real use cases
5. Update relevant documentation

**For Documentation:**
1. Use clear, concise language
2. Include code examples where helpful
3. Check spelling and grammar
4. Follow existing format

### Pull Request Process

1. **Fork the repository**
   ```bash
   gh repo fork ormus/hermetic-agents-pack
   ```

2. **Create a feature branch**
   ```bash
   git checkout -b feature/your-feature-name
   # or
   git checkout -b fix/bug-description
   ```

3. **Make your changes**
   - Follow existing code style
   - Write clear commit messages
   - Test your changes

4. **Commit with descriptive messages**
   ```bash
   git commit -m "Add: New mobile testing agent for Flutter"
   # or
   git commit -m "Fix: Improve backend-architect agent description"
   # or
   git commit -m "Docs: Add example for TikTok strategist workflow"
   ```

5. **Push to your fork**
   ```bash
   git push origin feature/your-feature-name
   ```

6. **Create pull request**
   - Use a clear, descriptive title
   - Reference related issues
   - Describe what changed and why
   - Include testing details
   - Add screenshots if relevant

### PR Title Format
```
[Type] Brief description

Types:
- Add: New feature or agent
- Fix: Bug fix
- Docs: Documentation only
- Style: Formatting, no code change
- Refactor: Code restructuring
- Test: Adding or updating tests
- Chore: Maintenance tasks
```

**Examples:**
```
Add: Performance optimization agent for database queries
Fix: Correct tool restrictions for frontend-developer agent
Docs: Add getting started tutorial for indie developers
```

---

## 🎨 Agent Design Guidelines

### Agent Structure

Every agent file should follow this structure:

```markdown
# Agent Name

**Specialization:** Clear one-line description

## When to Use This Agent

- Situation 1
- Situation 2
- Situation 3

## What This Agent Does

Detailed description of capabilities and expertise.

## Tools Available

- Tool 1
- Tool 2
- Tool 3

## Example Usage

### Example 1: [Scenario]
**Request:** "User's request"
**Agent Response:** What the agent will do

### Example 2: [Scenario]
**Request:** "User's request"
**Agent Response:** What the agent will do

## Best Practices

- Practice 1
- Practice 2
- Practice 3

## Limitations

- Limitation 1
- Limitation 2
```

### Agent Naming Conventions

- **Use clear, descriptive names**: "backend-architect" not "backend-guy"
- **Hyphen-separated**: "mobile-app-builder" not "MobileAppBuilder"
- **Lowercase**: "api-tester" not "API-Tester"
- **No abbreviations**: "user-experience-researcher" not "ux-res"

### Agent Descriptions

**Good description:**
> "Specialized in designing and implementing scalable RESTful APIs with authentication, database optimization, and server-side business logic. Focuses on Node.js, Python, and Go backends."

**Bad description:**
> "Helps with backend stuff"

### Tool Restrictions

Only include tools the agent actually needs:

**Backend Architect:**
```json
{
  "tools": ["Read", "Write", "Edit", "Bash", "Grep", "Glob"]
}
```

**UI Designer:**
```json
{
  "tools": ["Read", "Write", "Edit", "WebSearch", "WebFetch"]
}
```

Don't give all agents all tools!

---

## 🧪 Testing

### Before Submitting

**Test your changes:**
1. Install the plugin locally
2. Try the agent with real tasks
3. Verify automatic selection works
4. Test manual selection
5. Check error cases

**Agent testing checklist:**
- [ ] Agent activates correctly
- [ ] Automatic selection works for typical tasks
- [ ] Manual selection works
- [ ] Examples in description are accurate
- [ ] Tools are appropriate for the agent
- [ ] No conflicts with other agents

---

## 💬 Communication

### Be Respectful
- Assume good intentions
- Provide constructive feedback
- Welcome newcomers
- Celebrate contributions

### Response Times
- Maintainers typically respond within 48 hours
- Complex PRs may take longer to review
- Check back if no response after 1 week

### Getting Help
- Ask questions in GitHub Discussions
- Tag maintainers if urgent
- Join community channels

---

## 📋 Code of Conduct

### Our Pledge

We are committed to providing a welcoming and inspiring community for all.

**We will not tolerate:**
- Harassment of any kind
- Discrimination based on identity
- Trolling or insulting comments
- Personal or political attacks
- Publishing others' private information

**We encourage:**
- Respectful discourse
- Constructive feedback
- Helping newcomers
- Celebrating diverse perspectives

### Enforcement

Violations may result in:
1. Warning
2. Temporary ban
3. Permanent ban

Report issues to: ormus@hermetic.dev

---

## 🏆 Recognition

### Contributors

All contributors will be:
- Listed in CONTRIBUTORS.md
- Credited in release notes
- Thanked in the community

### Significant Contributions

Special recognition for:
- New agent creators
- Major feature additions
- Comprehensive documentation
- Long-term maintainers

---

## 📚 Resources

### Learn About the Project
- [README](README.md) - Project overview
- [CHANGELOG](CHANGELOG.md) - Version history
- [Examples](examples/) - Usage examples

### Learn About Claude Code
- [Claude Code Documentation](https://docs.claude.com/claude-code)
- [Plugin Development Guide](https://docs.claude.com/claude-code/plugins)
- [MCP Protocol](https://modelcontextprotocol.io/)

### Development Tools
- [GitHub CLI](https://cli.github.com/)
- [Git](https://git-scm.com/)
- [Markdown Guide](https://www.markdownguide.org/)

---

## 🎉 Thank You!

Every contribution, no matter how small, helps make this project better.

**Questions?**
- Open a [GitHub Discussion](https://github.com/ormus/hermetic-agents-pack/discussions)
- Join our community channels
- Reach out to maintainers

**Let's build something amazing together! 🚀**

---

**Last Updated:** 2025-10-12
**Version:** 1.0.0
