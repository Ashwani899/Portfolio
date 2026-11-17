# Ashwani Singhal - Portfolio

A responsive single-page portfolio built with semantic HTML, CSS custom properties, and vanilla JavaScript. The main experience lives in `index.html`; no frontend package installation or bundler is required.

## Portfolio sections

- **Profile and About:** Computer Science undergraduate at JUIT (2025-2029), technical interests, and current focus.
- **Selected Builds:** CONTROL-X (private research summary), ResumeForge AI, AI Study Assistant, EcoRoute AI, Jenkins Remoting, Azure CI/CD, Docker Web Server, Orbit Telemetry, JPMC Midas (Forage), and Techfest web experiences.
- **Architecture visuals:** source-grounded engineering flow diagrams for ResumeForge AI, AI Study Assistant, and the high-level CONTROL-X evaluation loop. These are diagrams, not fabricated product screenshots.
- **GitHub Profile & Activity:** GitHub avatar, public profile-statistics cards, language distribution, and a third-party contribution-calendar visualisation.
- **Skills & Tools:** grouped technologies represented in public project repositories and learning work.
- **Certifications:** existing verification links retained in the HTML.
- **Experience & Programmes:** CodeAlpha, 1M1B/AICTE/IBM SkillsBuild, GeeksforGeeks, Techfest, and Aspire Institute.
- **Résumé:** embedded previews and downloadable one-page PDFs for Software Engineering and AI/ML roles.
- **Contact:** GitHub, LinkedIn, LeetCode, and email.

## Résumé downloads

- [Software Engineering résumé (PDF)](assets/Ashwani_Singhal_Software_Engineering_Resume_2026.pdf)
- [AI/ML Engineering résumé (PDF)](assets/Ashwani_Singhal_AI_ML_Resume_2026.pdf)

Both PDFs are A4, one page, and use role-specific summaries and project ordering. The CONTROL-X description is explicitly scoped as ongoing private research; it does not claim confirmatory effectiveness results or a certified false-positive estimate.

## Built with

- HTML5, CSS, and vanilla JavaScript.
- Space Grotesk, IBM Plex Sans, and IBM Plex Mono via Google Fonts.
- `IntersectionObserver` for scroll reveal and navigation state.
- Responsive CSS layouts, keyboard-visible focus styles, and reduced-motion support.
- Inline engineering flow diagrams and native browser PDF previews.

## Selected public repositories

| Project | Repository |
|---|---|
| EcoRoute AI - uncertainty-aware waste-routing prototype | [GitHub](https://github.com/Ashwani899/EcoRoute-AI-Component-Aware-Uncertainty-Gated-Waste-Routing-System) |
| ResumeForge AI - deterministic resume analysis and tailoring | [GitHub](https://github.com/Ashwani899/resumeforge-ai) |
| AI Study Assistant - document-grounded learning workflows | [GitHub](https://github.com/Ashwani899/ai-study-assistant) |
| Jenkins Remoting Lab - distributed agent learning lab | [GitHub](https://github.com/Ashwani899/Jenkins-Remoting-Project) |
| Azure CI/CD Pipeline - Flask/Docker application and Azure Pipelines definition | [GitHub](https://github.com/Ashwani899/Azure-CI-CD-pipeline-from-scratch) |
| Docker Web Server - Nginx containerization | [GitHub](https://github.com/Ashwani899/Docker-webserver-project) |
| Orbit Telemetry - Java service and observability prototype | [GitHub](https://github.com/Ashwani899/Java-Application-using-Gradle-) |
| JPMC Midas - Forage virtual-experience exercise | [GitHub](https://github.com/Ashwani899/forage-midas/tree/flow) |
| Techfest 3D - interactive event-site experience | [GitHub](https://github.com/Ashwani899/Techfest-3D) |
| Techfest Synthesis - interactive candidate experience | [GitHub](https://github.com/Ashwani899/Techfest-Synthesis) |

**Accuracy notes**

- CONTROL-X is an ongoing private research project. The public summary intentionally omits private code, frozen baselines, preregistered settings, experimental data, and unpublished findings.
- The Azure repository contains an Azure Pipelines definition. GitHub Actions validation does not establish a successful live Azure deployment; that requires configured Azure resources and service connections.
- The Jenkins repository is a learning lab and configuration reference, not a production Jenkins service.
- JPMC Midas is a learner exercise associated with the JPMorgan Chase & Co. Advanced Software Engineering virtual experience on Forage; it is not JPMorgan Chase production software or employment.
- GitHub statistics and the contribution calendar are third-party visualisations and may be cached or unavailable. GitHub itself is authoritative for contribution attribution and account activity.

## Local preview

Open `index.html` directly in a modern browser, or start a local server:

```bash
python -m http.server 8000
```

Then open `http://localhost:8000`.

## Validation

The `.github/workflows/portfolio-validation.yml` workflow runs `scripts/validate_portfolio.py` on pull requests and pushes. It checks internal anchors, duplicate IDs, placeholder copy, and the presence and one-page structure of both PDF résumés.

## GitHub profile README

`GITHUB_PROFILE_README_DRAFT.md` is the prepared profile README. GitHub displays it when a public repository named exactly `Ashwani899` contains a root `README.md`. That special repository still needs to be created and populated; this draft in the Portfolio repository does not itself appear on the profile page.

## Deployment

The changes in this branch are not live until the pull request is reviewed, merged, and the GitHub Pages deployment succeeds. Check [Actions](https://github.com/Ashwani899/Portfolio/actions) for the post-merge result and **Settings -> Pages** for the canonical URL.
