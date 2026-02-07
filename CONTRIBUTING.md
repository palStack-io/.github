# Contributing to palStack

Thanks for your interest in contributing to palStack! We're building privacy-first life management tools that actually respect your data and your time. Whether you're fixing a typo or adding a major feature, we appreciate your help.

## Our Philosophy

**"Pals show up and help with the everyday stuff."**

## Core Team

- **Harun Gunasekaran** - Founder & Lead Developer
- **Rachel Surette** - Co-Founder, Marketing & Sustainability
- **Elle Russell** - Co-Founder, Lead UI/UX Designer
- **Chris Macioci** - Co-Founder, Lead DevOps
- **Chaitanya Gunupudi** - Senior Advisor, Cybersecurity & DevOps *(open-source repos only)*

---

## What Can You Contribute To?

### Public Repositories (Open Source - AGPL-3.0)
These are fully open for community contributions:

- [**pantrypal-core**](https://github.com/palStack-io/pantrypal-core) - Food waste reduction through pantry management
- [**propertypal-core**](https://github.com/palStack-io/propertypal-core) - Home maintenance tracking
- [**clubpal-core**](https://github.com/palStack-io/clubpal-core) - Group coordination for dining and activities  
- [**finpal-core**](https://github.com/palStack-io/finpal-core) - Budget tracking


### Private Repositories (Team Only)
These are currently private and not accepting external contributions:

- Mobile apps (React Native/Expo)
- Premium features
- Managed hosting infrastructure
- palStack Web - Marketing website and documentation

We keep mobile apps private during development but may open-source them later. If you're interested in mobile development, reach out to discuss potential collaboration.

---

## How to Contribute

### 1. Find Something to Work On

**Good first contributions:**
- Fix typos in documentation
- Improve error messages
- Add tests for existing features
- Update README or setup instructions
- Report bugs with clear reproduction steps

**Check these places:**
- Issues labeled `good first issue`
- Issues labeled `help wanted`
- Documentation that needs clarification
- Features marked `accepting-contributions` in our roadmap

**Not sure what to work on?** Open an issue and ask! We're happy to suggest something that matches your skills and interests.

---

### 2. Set Up Your Development Environment

#### Prerequisites
```bash
# For backend services (Python/FastAPI)
python >= 3.11
docker >= 24.0
docker-compose >= 2.20

# For web frontend (React/Vite)
node >= 18.0
npm >= 9.0
```

#### Quick Start
```bash
# 1. Fork the repository on GitHub
# 2. Clone your fork
git clone git@github.com:YOUR_USERNAME/REPO_NAME.git
cd REPO_NAME

# 3. Add upstream remote
git remote add upstream git@github.com:palStack-io/REPO_NAME.git

# 4. Install dependencies and run
# For Python services:
docker-compose up -d

# For Node.js/React:
npm install
npm run dev
```

#### Keeping Your Fork Updated
```bash
git fetch upstream
git checkout main
git merge upstream/main
git push origin main
```

---

### 3. Make Your Changes

**Create a branch:**
```bash
git checkout -b feature/your-feature-name
# or
git checkout -b fix/bug-description
```

**Branch naming conventions:**
- `feature/` - New features
- `fix/` - Bug fixes
- `docs/` - Documentation changes
- `refactor/` - Code refactoring
- `test/` - Adding tests
- `chore/` - Maintenance tasks

**Write good commits:**
```bash
git commit -m "feat(pantrypal): add expiration notifications

- Add background job to check expiring items
- Send email notifications 3 days before expiry
- Add user preference for notification timing

Fixes #123"
```

**Commit message format:**
```
type(scope): brief description

- Detailed change 1
- Detailed change 2
- Detailed change 3

Fixes #issue-number
```

**Types:** `feat`, `fix`, `docs`, `style`, `refactor`, `test`, `chore`, `security`, `perf`

---

### 4. Test Your Changes

**Before submitting, make sure:**
- [ ] Code follows existing patterns and style
- [ ] You've tested locally (Docker Compose or `npm run dev`)
- [ ] No console errors or warnings
- [ ] Docker image builds successfully (if applicable)
- [ ] Tests pass (if tests exist)
- [ ] Documentation updated (if needed)

**Run tests:**
```bash
# Python services
docker-compose exec SERVICE_NAME pytest

# Node.js/React
npm run test
npm run lint
```

---

### 5. Submit a Pull Request

**Push your branch:**
```bash
git push origin feature/your-feature-name
```

**Create PR on GitHub:**
1. Go to the original repository
2. Click "Pull requests" → "New pull request"
3. Click "compare across forks"
4. Select your fork and branch
5. Fill out the PR template (it'll appear automatically)
6. Submit!

**PR Guidelines:**
- One feature/fix per PR (easier to review)
- Link related issues
- Include screenshots for UI changes
- Be honest about AI assistance (we use it too!)
- Explain your reasoning for architectural decisions

---

## Code Style & Standards

### Python (FastAPI Services)

**Follow these patterns:**
```python
# Use type hints
def create_item(name: str, quantity: int) -> dict:
    return {"name": name, "quantity": quantity}

# Use descriptive names
def calculate_expiration_date(purchase_date, shelf_life_days):
    # Good: Clear what this does
    pass

# Keep functions focused
def validate_and_save_item(item):
    # Better: Split into validate_item() and save_item()
    pass
```

**Standards:**
- Use `black` for formatting (or follow existing style)
- Type hints for function parameters and returns
- Docstrings for complex functions
- No hardcoded credentials (use environment variables)
- SQL parameterization (no string interpolation)

### JavaScript/React (Web & Mobile)

**Follow these patterns:**
```javascript
// Use descriptive component names
function PantryItemCard({ item, onDelete }) {
  // Good: Clear what this component does
}

// Keep components focused
function UserProfilePage() {
  // If this is doing too much, split it
}

// Use meaningful variable names
const expiringItems = items.filter(item => item.daysUntilExpiry <= 3);
```

**Standards:**
- Functional components with hooks (not classes)
- Props validation with PropTypes or TypeScript
- Accessibility attributes (ARIA labels, semantic HTML)
- Mobile-first responsive design
- Follow existing Tailwind patterns

### Docker & Infrastructure

**Follow these patterns:**
- Multi-stage builds to minimize image size
- Non-root users in containers
- Health checks in docker-compose
- Environment variables for configuration
- Clear comments for complex commands

---

## Security

**Never commit:**
- API keys or passwords
- Access tokens
- Private keys
- User data
- `.env` files with secrets

**If you accidentally commit secrets:**
1. Immediately revoke/rotate the credentials
2. Tell us in the PR 
3. We'll help clean up the git history

**Report security issues privately:**
Email: palstack4u@gmail.com or harung1993@gmail.com (don't open public issues)

We'll respond within 48 hours and credit you in our changelog.

---

## AI-Assisted Contributions

**We're transparent about AI use.** If you used Claude, ChatGPT, GitHub Copilot, or other AI tools:

- Do disclose it in your PR - Check the "AI-assisted" box in the PR template
- Do review and understand the code - You should be able to explain what it does
- Do test thoroughly - AI makes mistakes
- Do modify for our patterns - AI doesn't know palStack conventions

**Our policy:**
- AI suggestions are welcome
- Human review is required
- You're responsible for code you submit (AI or not)
- Security-sensitive code gets extra scrutiny

---

## Getting Help

**Stuck? Need clarification?**

1. **Check existing docs** - README, wiki, comments
2. **Search closed issues** - Someone may have asked before
3. **Join our Discord** - Ask questions at [discord.gg/qQUszVa7km](https://discord.gg/qQUszVa7km)
4. **Open an issue** - For bugs or feature discussions
5. **Ping maintainers** - @mention us in comments

**We promise:**
- No question is too basic
- We won't make you feel stupid
- We'll respond within a few days
- If something's unclear, that's on us to fix

---

## Recognition

**We value contributors:**
- Your name in CONTRIBUTORS.md
- Shout-out in release notes for major contributions
- Early access to new features (if you want)
- Our genuine gratitude

---

## Code of Conduct

**Be excellent to each other:**

- Be kind and respectful
- Welcome newcomers
- Focus on ideas, not people
- Assume good intent
- No harassment, discrimination, or toxicity


---

## License

By contributing to palStack, you agree that your contributions will be licensed under the same license as the project:

- **Open-source repos:** AGPL-3.0
- **Documentation:** CC BY 4.0

Your contributions remain yours, but you grant us permission to use them in palStack.

---

## Questions?

- **General questions:** Join our [Discord community](https://discord.gg/qQUszVa7km)


---

**Thanks for contributing! Let's build something useful together.**
