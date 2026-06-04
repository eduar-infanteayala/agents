# agents

## Plan for skills and agent capabilities

This repository can be used as a simple planning reference for choosing the right skill or agent based on the job to be done.

### 1. Skills plan

| Skill | When to use it | Primary outcome |
| --- | --- | --- |
| `customize-cloud-agent` | When you need to configure the cloud agent environment, install dependencies, or define setup steps | A ready-to-use agent environment for the rest of the work |

### 2. Agent capabilities plan

| Agent | Core capability | Best-fit use cases |
| --- | --- | --- |
| `explore` | Fast repository and codebase discovery | Understanding project structure, locating files, tracing features, gathering technical context |
| `task` | Reliable command execution | Running tests, builds, linters, and other verification commands |
| `general-purpose` | End-to-end implementation work | Multi-step feature work, bug fixing, refactoring, and coordinated documentation updates |
| `code-review` | High-signal review of code changes | Reviewing pull requests, finding bugs, security issues, and risky logic changes |
| `research` | Deep external or cross-repository investigation | Comparing approaches, checking upstream examples, and gathering references before implementation |

### 3. Use-case mapping

| Your use case | Recommended skill/agent | Reason |
| --- | --- | --- |
| Set up the working environment | `customize-cloud-agent` | Prepares tools, dependencies, and runner behavior before coding starts |
| Learn how a repository works | `explore` | Optimized for fast inspection and discovery |
| Run validation after changes | `task` | Best for focused execution of tests, builds, and linters |
| Implement a feature or fix | `general-purpose` | Handles multi-step reasoning and code changes well |
| Review a branch before merging | `code-review` | Focuses on meaningful defects instead of style noise |
| Research options before deciding | `research` | Useful for evidence-based technical decisions |

### 4. Recommended workflow

1. Start with `customize-cloud-agent` if the environment needs setup.
2. Use `explore` to understand the codebase or request.
3. Use `general-purpose` for implementation work.
4. Use `task` to validate with existing tests, builds, or linters.
5. Use `code-review` before merging important changes.
6. Use `research` when the decision depends on outside references or comparisons.

### 5. Decision rule

- If the problem is **understanding**, use `explore`.
- If the problem is **executing commands**, use `task`.
- If the problem is **building or changing something**, use `general-purpose`.
- If the problem is **checking quality or risk**, use `code-review`.
- If the problem is **finding evidence or examples**, use `research`.
- If the problem is **preparing the environment**, use `customize-cloud-agent`.
