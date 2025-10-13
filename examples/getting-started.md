# Getting Started with Hermetic Agents Pack

Welcome! This guide will help you start using the Hermetic Agents Pack effectively.

---

## 🚀 Quick Start (5 Minutes)

### Step 1: Install the Plugin

```bash
/plugin install hermetic-agents-pack
```

You should see:
```
✅ Hermetic Agents Pack installed! 39 specialized agents are now available.
   Claude will automatically delegate to the right agent for your tasks.
```

### Step 2: Verify Installation

All agents are automatically loaded. No configuration needed!

###Step 3: Try Your First Agent

**Automatic selection (recommended):**
```
"Design a landing page for a meditation app"
```

Claude automatically selects the **UI Designer** agent.

**Manual selection:**
```
"Use the ui-designer agent to create a landing page for a meditation app"
```

---

## 🎯 Common Use Cases

### Building a New Feature

**Scenario:** Add social sharing to your app

**What to say:**
```
"Add social sharing functionality with Twitter, Facebook, and TikTok.
Include share buttons, preview cards, and analytics tracking."
```

**Agents involved:**
- **Frontend Developer** - Share button UI components
- **Backend Architect** - Share tracking API
- **TikTok Strategist** - Optimize for TikTok sharing
- **Test Writer/Fixer** - Test suite for sharing feature

**Expected outcome:**
- Complete implementation plan
- Code for all components
- Tests included
- Best practices applied

---

### Planning a Sprint

**Scenario:** Plan next week's development

**What to say:**
```
"Help me plan a 6-day sprint. I have:
- User authentication (high priority)
- Push notifications (medium priority)
- Dark mode (nice to have)
My team: 2 developers, 1 designer. Budget: 40 hours."
```

**Agents involved:**
- **Sprint Prioritizer** - Create prioritized plan
- **Studio Producer** - Resource allocation
- **Backend Architect** - Technical complexity assessment

**Expected outcome:**
- Prioritized sprint backlog
- Day-by-day breakdown
- Risk assessment
- Resource allocation

---

### Launching an App

**Scenario:** Prepare for App Store launch

**What to say:**
```
"I'm launching my fitness app next week. Help me prepare everything:
App Store listing, launch content, support setup, and analytics."
```

**Agents involved:**
- **App Store Optimizer** - Store listing optimization
- **TikTok Strategist** - Launch content strategy
- **Project Shipper** - Launch coordination
- **Support Responder** - Support documentation
- **Analytics Reporter** - Metrics dashboard setup

**Expected outcome:**
- Complete launch checklist
- Optimized App Store listing
- Content calendar
- Support documentation
- Analytics setup

---

### Improving Quality

**Scenario:** Make app faster and more delightful

**What to say:**
```
"My app feels slow and lacks personality. Help me:
1. Profile and optimize performance
2. Add delightful micro-interactions
3. Improve loading states"
```

**Agents involved:**
- **Performance Benchmarker** - Profiling and optimization
- **Whimsy Injector** - Delightful interactions
- **Frontend Developer** - Implementation
- **Test Writer/Fixer** - Performance tests

**Expected outcome:**
- Performance audit report
- Optimization recommendations
- Delightful interaction ideas
- Implementation code
- Performance tests

---

## 🎨 Agent Categories Quick Reference

### When You Need...

**Backend work:**
→ Backend Architect, API Tester, DevOps Automator

**Frontend work:**
→ Frontend Developer, UI Designer, Whimsy Injector

**Mobile features:**
→ Mobile App Builder, Performance Benchmarker

**Design:**
→ UI Designer, UX Researcher, Brand Guardian, Visual Storyteller

**Testing:**
→ Test Writer/Fixer, Performance Benchmarker, API Tester

**Marketing:**
→ TikTok Strategist, App Store Optimizer, Trend Researcher

**Product:**
→ Sprint Prioritizer, Feedback Synthesizer, UX Researcher

**Operations:**
→ Analytics Reporter, Finance Tracker, Infrastructure Maintainer

**Launch:**
→ Project Shipper, App Store Optimizer, Support Responder

---

## 💡 Pro Tips

### Tip 1: Be Specific

**❌ Vague:**
```
"Make my app better"
```

**✅ Specific:**
```
"Optimize my app's initial load time. Currently takes 5 seconds,
target is under 2 seconds. Using React Native with Redux."
```

### Tip 2: Provide Context

**❌ No context:**
```
"Add authentication"
```

**✅ With context:**
```
"Add OAuth authentication for a social app with 10k users.
Support Google and GitHub login. Need secure token management
and automatic token refresh."
```

### Tip 3: Let Claude Choose

Don't always specify the agent manually. Claude is smart about selecting the right one:

**Good:**
```
"Design and implement a user onboarding flow"
```

**Also Good (but unnecessary):**
```
"Use the ui-designer agent to design and the frontend-developer
agent to implement a user onboarding flow"
```

### Tip 4: Multi-Agent Tasks

For complex tasks, describe the full scope:

```
"Build a complete authentication system:
- OAuth with Google/GitHub (backend)
- Login UI (frontend)
- User profile management (full-stack)
- Security audit
- Test coverage"
```

Claude will coordinate multiple agents automatically.

### Tip 5: Iterative Refinement

Start broad, then refine:

1. **First:**
```
"Design a meditation app"
```

2. **Then:**
```
"Make the meditation timers more engaging"
```

3. **Finally:**
```
"Add subtle breathing animation to the timer"
```

---

## 🛠️ Troubleshooting

### Agent Not Responding as Expected

**Problem:** Agent doesn't seem to be working correctly

**Solutions:**
1. **Be more specific** in your request
2. **Explicitly name the agent** you want
3. **Provide more context** about your project
4. **Break down complex requests** into steps

**Example:**

Instead of:
```
"Fix my app"
```

Try:
```
"Use the performance-benchmarker agent to profile my React app
and identify why the dashboard takes 3+ seconds to load"
```

### Wrong Agent Selected

**Problem:** Claude selected a different agent than you expected

**Solutions:**
1. **Manually specify the agent:**
```
"Use the backend-architect agent to..."
```

2. **Provide clearer context:**
```
"For the server-side API implementation, design..."
```

3. **The agent will adapt** - Even if slightly wrong, agents can handle related tasks

### Need Multiple Agents

**Problem:** Task needs expertise from several agents

**Solutions:**
1. **Describe the full scope:**
```
"Build feature X with frontend, backend, tests, and documentation"
```

2. **Request sequentially:**
```
"First, use backend-architect to design the API"
(wait for response)
"Now, use frontend-developer to build the UI"
```

3. **Let Claude coordinate:**
```
"Complete implementation of feature X including all aspects"
```

---

## 📚 Learning Resources

### Agent Documentation

Each agent has detailed documentation in their respective files:

```
agents/
├── engineering/
│   ├── backend-architect.md       ← Read this for backend tasks
│   ├── frontend-developer.md      ← Read this for frontend tasks
│   └── ...
├── design/
│   ├── ui-designer.md             ← Read this for UI tasks
│   └── ...
└── ...
```

### Example Workflows

**Full-Stack Feature:**
```
"Build a comment system:
- Backend API with moderation
- React component for comments
- Real-time updates with WebSocket
- Spam detection
- Test coverage"
```

**App Launch:**
```
"Launch my habit tracking app:
- Optimize App Store listing
- Create TikTok launch content
- Set up analytics
- Prepare support docs
- Schedule launch activities"
```

**Performance Optimization:**
```
"My app is slow:
- Profile the performance
- Identify bottlenecks
- Implement optimizations
- Add performance tests
- Verify improvements"
```

---

## 🎯 Next Steps

### 1. Try Each Agent Category

Spend a few minutes with each:
- Engineering agents
- Design agents
- Marketing agents
- Testing agents
- Operations agents

### 2. Build Something Real

Use the agents for an actual project:
- Start small (one feature)
- Use automatic delegation
- Learn agent strengths
- Iterate based on results

### 3. Develop Your Workflow

Find patterns that work for you:
- Morning planning with Sprint Prioritizer
- Feature development with Engineering agents
- Quality checks with Testing agents
- Deployment with DevOps Automator

### 4. Share Your Experience

Help improve the pack:
- Report issues
- Suggest improvements
- Share success stories
- Contribute examples

---

## 💬 Get Help

**Questions?**
- [GitHub Discussions](https://github.com/ormus/hermetic-agents-pack/discussions)
- [Discord/Slack Community]
- [Documentation](../docs/)

**Found a bug?**
- [GitHub Issues](https://github.com/ormus/hermetic-agents-pack/issues)

**Want to contribute?**
- [Contributing Guide](../CONTRIBUTING.md)

---

## 🎉 You're Ready!

Start building with your complete AI agent team.

**Your first command:**
```
"Help me build [your idea]"
```

**Let the agents do what they do best!** 🚀

---

**Happy building!**

---

**Last Updated:** 2025-10-12
**Plugin Version:** 1.0.0
