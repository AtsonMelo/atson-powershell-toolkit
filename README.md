# Atson PowerShell Toolkit

## What It Does

Professional PowerShell automation toolkit for Windows system administration, productivity workflows, and technical scripting. Provides reusable scripts, utilities, and best practices for Microsoft Graph integration, file synchronization, markdown-based documentation, and secure operational workflows.

---

## Why It Exists

Professional Windows automation requires:
- Clean, reusable script patterns
- Secure credential and secret handling
- Integration with Microsoft services (Graph API, Office 365)
- Local network synchronization capabilities
- Centralized logging and documentation
- Examples and templates for common tasks

This toolkit captures these patterns and makes them easy to use and extend.

---

## Features

- ✓ Microsoft Graph API integration
  - Email sending and scheduling
  - Calendar event creation
  - User and resource management
  - Token-based authentication
- ✓ Local network synchronization
  - Robocopy-based file sync
  - Scheduled sync workflows
  - Progress logging
- ✓ Markdown-based documentation
  - Note-taking automation
  - Evidence collection
  - Technical logs
- ✓ Secure credential management
  - VeraCrypt integration patterns
  - Secure credential storage
  - Vault examples
- ✓ System administration utilities
  - Common Windows automation tasks
  - Best practices and examples
  - Well-documented templates

---

## Tech Stack

- **Language:** PowerShell 5.1+
- **Platform:** Windows 10+
- **APIs:** Microsoft Graph API, Office 365
- **Tools:** Git, GitHub, VeraCrypt, Robocopy
- **Documentation:** Markdown, examples

---

## Project Status

**Status:** Active / Work in Progress  
**Phase:** Ongoing development and refinement  
**Last Updated:** May 2026

This is a growing collection of production-ready and experimental automation scripts. New utilities are added as needed.

---

## How to Use

### Prerequisites

- Windows 10 or later
- PowerShell 5.1 or later (PowerShell 7+ recommended)
- .NET Framework or .NET Core (for some operations)
- Git

### Installation

```powershell
# Clone the repository
git clone https://github.com/AtsonMelo/atson-powershell-toolkit.git
cd atson-powershell-toolkit

# Review available scripts
Get-ChildItem *.ps1 | Format-List Name, Description

# Execute a script
.\script-name.ps1
```

### Module Usage

Import specific modules:

```powershell
# Import Graph utilities
Import-Module .\modules\MicrosoftGraph.psm1

# List available functions
Get-Command -Module MicrosoftGraph
```

### Project Structure

```
atson-powershell-toolkit/
├── scripts/                      # Individual automation scripts
│   ├── microsoft-graph/          # Graph API examples
│   ├── sync/                     # Sync utilities
│   ├── notes/                    # Markdown documentation
│   └── admin/                    # System administration
├── modules/                      # Reusable PowerShell modules
├── templates/                    # Script templates
├── docs/                         # Documentation and guides
└── README.md
```

---

## Features & Roadmap

### Completed

- [x] Microsoft Graph authentication and token handling
- [x] Email sending via Graph API
- [x] Calendar event automation
- [x] Robocopy-based sync scripts
- [x] Markdown note-taking utilities
- [x] Security patterns and examples

### Planned / In Progress

- [ ] Azure CLI integration
- [ ] Advanced scheduling and task automation
- [ ] Metrics and reporting dashboards
- [ ] Event-driven automation patterns
- [ ] Cloud storage integration (OneDrive, SharePoint)
- [ ] Workflow orchestration examples

---

## Security & Privacy

⚠️ **Critical:**
- **Never commit credentials, tokens, or secrets**
- **Never include API keys or authentication strings**
- **Never commit real VeraCrypt vaults or password files**
- **Never log sensitive data (PII, financial info, credentials)**
- **Use .gitignore for all configuration files with real values**
- **Test credential handling before running in production**

### Safe Patterns

This toolkit includes examples of:
- Secure credential storage and retrieval
- Token-based authentication
- Credential prompt patterns
- Logging without exposing secrets

---

## Contributing

This is a personal portfolio project. For improvements or suggestions:

1. Open an issue for feature requests or bug reports
2. Feel free to fork and experiment
3. Submit PRs for documentation or example improvements

---

## License

**License:** Pending decision  
Currently no explicit license. If you plan to use this code, ask for clarification on licensing terms.

---

## Author

**Atson Melo**  
Focus: PowerShell automation, system administration, productivity workflows  
Interests: Microsoft ecosystem, Azure, automation frameworks  
GitHub: [@AtsonMelo](https://github.com/AtsonMelo)

---

## Related Projects

- [monitor-hardware](https://github.com/AtsonMelo/monitor-hardware) – Hardware monitoring and diagnostics
- [monitor-com](https://github.com/AtsonMelo/monitor-com) – Serial communication monitoring
- [testador-neon-hio115](https://github.com/AtsonMelo/testador-neon-hio115) – Industrial testing tool
