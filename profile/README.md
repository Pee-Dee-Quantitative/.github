# Pee Dee Quantitative

Building **data-driven systems for quantitative research and trading**.

---

## Organization Overview

Pee Dee Quantitative develops propertiery systems and libraries for algorithmic trading, data engineering, and quantitative research.  
Our naming, design, and culture are inspired by the **heritage, nature, and innovation of South Carolina**.

---

## Repository Naming Convention

Our repositories are grouped by **theme** and **purpose**, following South Carolina’s culture and natural symbols.

| Category              | Emoji | Theme                          | Purpose                                               | Example Repos                                 |
| --------------------- | :---: | ------------------------------ | ----------------------------------------------------- | --------------------------------------------- |
| **Core Systems**          | 🌳 | Plants / Strong Flora          | Core quant engines, domain logic, strategy systems    | `Palmetto/`, `Dogwood/`, `Sassafras/`, `Magnolia/` |
| **Research**              | 🐦 | Fauna / State Wildlife         | Research notebooks, prototypes, experiments           | `BoykinSpaniel/`, `IndigoBunting/`, `Loggerhead/` |
| **Infrastructure**        | 💎 | Minerals / Gemstones           | Logging, metrics, storage, CI/CD                      | `Amethyst/`, `Garnet/`, `Quartz/`, `Onyx/` |
| **Documentation**         | 🏞 | Landmarks / Rivers / Lakes     | Architecture, guides, contribution, roadmap           | `Congaree/`, `Savannah/`, `PaulWallace/`, `Ashley/` |
| **Utilities**             | 🏘 | Small Towns / Cultural Centers | Helper tools, CLIs, shared libs, automation           | `Clio/`, `Tatum/`, `Bennettsville/`, `Smyrna/` |
| **Data Systems**          | 🧠 | Inventions / Inventors         | Historical data, backtesting, market feeds, data prep | `Townes/`, `Coker/`, `Murray/`, `Seibels/`, `Blenheim/` |
| **Security / Governance** | 🛡 | Fortifications / Patriots      | Security policies, auditing, access control           | `FortSumter/`, `SwampFox/`, `CastlePinckney/` |

---

## Branching Strategy

We follow a **trunk-based development** approach.  
Our main branch (`main`) is protected — direct commits are not allowed except in emergencies.

### Branch Naming Convention

Format: category/issueNumber-brief-description
Examples:  
- `feat/45-add-vwap-indicator`  
- `chore/7-update-gitignore`

Each branch should correspond to **one GitHub Issue** (or sub-issue).  
If the issue is large, create sub-issues and branch off accordingly.
Use lowercase with a hypen to seperate words.
The issueNumber should be in front after the category and slash.

### Branch Categories
| Type | Purpose |
|------|----------|
| **feat** | New feature |
| **fix** | Bug fix |
| **docs** | Documentation changes |
| **refactor** | Code restructure (no functional change) |
| **test** | Adding or modifying tests |
| **chore** |Minor maintenance, build scripts, formatting, or general project upkeep |
| **security** | Cybersecurity updates |
| **infra** | Infrastructure tasks like CI/CD, observability, feature flags, and automation setup |

### General Conventions

- Keep changes **small, focused, and atomic**.  
- A branch should typically **live less than a day**.  
- Old branches are **purged periodically**.  
- All new functionality should be **protected by feature flags**.  
- After merging, test changes in the **dev environment**.  
- Code in `main` should always be **deployable** — if it’s not ready, don’t merge it.  

---

## Commit Conventions

You can commit as frequently as needed.  
For the **final commit before PR**, use a descriptive message with issue references, such as:
fix(#101): handle null response from Alpaca

---

##  Example Workflow
1. Create an issue or sub-issue in GitHub.  
2. Branch from `main` using the correct naming convention.  
3. Develop locally and commit changes incrementally.  
4. Open a Pull Request with a clear description and link to the issue.  
5. Once approved, merge into `main` and verify in the dev environment.
