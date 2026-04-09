# opencell-tools

A collection of Claude Code plugins that streamline the OpenCell developer workflow — from Jira ticket management and UI scaffolding to automated commits, pull requests, and code review.

## Installation

```bash
claude
/install-plugin marketplace https://github.com/mhamidi81/ccode-marketplace.git
```

## Plugins

### Skills (slash commands)

| Plugin | Command | Description |
|--------|---------|-------------|
| **oc-cache-jira** | `/cache-jira` | Fetch and cache Jira ticket data locally for use by other commands |
| **oc-commit** | `/oc-commit` | Commit changes using the cached Jira ticket ID and summary with automatic code review |
| **oc-pull-request** | `/oc-pr` | Push changes and create a pull request for the current Jira ticket |
| **oc-create-ui** | `/oc-create-ui` | Scaffold a UI page from a Jira ticket using the frontend-engineer sub-agent |
| **oc-fix-bug** | `/oc-fix-bug` | Fix a bug from a Jira ticket — update status to In Progress, create fix branch, and start fixing |
| **oc-review-pr** | `/oc-review-pr` | Review a pull request linked to a Jira ticket — fetch PR, select appropriate reviewer agent, and generate a detailed report |

### Sub-agents

| Plugin | Description |
|--------|-------------|
| **oc-frontend-engineer** | Expert React/TypeScript sub-agent for building, refactoring, and architecting frontend components |
| **oc-frontend-designer** | Frontend designer sub-agent for translating Figma designs into implementation-ready React/MUI components with design tokens and styling |
| **oc-frontend-reviewer** | Frontend code reviewer sub-agent that validates React/TypeScript code against project standards |
| **oc-core-reviewer** | Backend code reviewer sub-agent for validating Java/EJB/JPA/Liquibase code against Opencell core project standards |
| **oc-cypress-expert** | Cypress testing expert sub-agent for end-to-end testing, test automation, and flaky test resolution |

### MCP Integrations

| Plugin | Description |
|--------|-------------|
| **oc-bitbucket-mcp** | Create pull requests, manage repositories, and review code on Bitbucket |
| **oc-figma-mcp** | Extract design context, generate code from Figma designs, and retrieve design tokens |
| **oc-playwright-mcp** | Automate browser interactions, take screenshots, and test web applications |
| **oc-opencell-mcp** | Query and manage the Opencell billing system — invoices, quotes, customers, payments, subscriptions, and more |
| **oc-sonar-mcp** | Access SonarQube code quality metrics, issues, and analysis results |
| **oc-postgres-mcp** | Database health analysis, index tuning, query optimization, and safe SQL execution via PostgreSQL |
