# AIP-Guardian Architecture

## Repository Structure

```
aip-guardian/
├── index.html          # Main entry point (GitHub Pages root)
├── README.md           # Project documentation
├── docs/
│   └── MISSION.md      # AIP Mission document
└── deep/
    ├── OVERVIEW.md     # Architectural overview
        ├── ARCHITECTURE.md # This file
            └── ROADMAP.md      # Future roadmap
            ```

            ## Deployment Architecture

            ```
            GitHub Repository (main branch)
                    │
                            ▼
                            GitHub Pages Build
                                    │
                                            ▼
                                            https://racinc19.github.io/aip-guardian/
                                                    │
                                                            ▼
                                                            index.html (served as root)
                                                            ```

                                                            ## Technology Stack

                                                            | Layer | Technology |
                                                            |-------|-----------|
                                                            | Hosting | GitHub Pages |
                                                            | Source Control | GitHub (main branch) |
                                                            | Frontend | HTML5, CSS3 |
                                                            | Documentation | Markdown (.md) |
                                                            | CI/CD | GitHub Actions (Pages workflow) |

                                                            ## Design Decisions

                                                            ### Static Site
                                                            The project uses a static HTML/CSS approach for maximum compatibility, zero dependencies, and instant deployment via GitHub Pages.

                                                            ### Flat Structure
                                                            Files are organized at the root level for GitHub Pages compatibility. The `index.html` serves as the primary entry point.

                                                            ### Documentation Hierarchy
                                                            - Root `README.md`: Project overview
                                                            - `docs/`: Mission-level documentation
                                                            - `deep/`: Technical deep-dive documentation

                                                            ## Security

                                                            - HTTPS enforced via GitHub Pages
                                                            - No server-side code — fully static
                                                            - No user data collected
                                                            - Open source — fully auditable
