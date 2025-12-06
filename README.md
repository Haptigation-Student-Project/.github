# Organization-wide Templates and Guidelines

This repository provides organization-wide GitHub guidelines and templates. It includes community health files, standard issue and pull request templates, shared workflows, and the organization profile. Content in `.github` can apply to all repositories in the organization without being duplicated in each project.

## Contents and Structure

- `profile/README.md`
	- Organization profile page on GitHub. Displayed on the organization page and communicates mission, projects, links, and notes.
- `assets/`
	- Static resources (images, badges, logos) referenced in profiles/READMEs/templates.
- Community health files (optional, recommended):
	- `CODE_OF_CONDUCT.md` – Code of conduct for all contributions in the organization.
	- `SECURITY.md` – Security notes and reporting channels for vulnerabilities.
	- `SUPPORT.md` – How and where support can be obtained.
- Templates (optional, recommended):
	- `ISSUE_TEMPLATE/` – One or more issue templates (bug, feature, question).
	- `PULL_REQUEST_TEMPLATE.md` – Consistent PR checklist and description.
    - `USER_STORY_TEMPLATE.md` – How to write a proper user story.
- Workflows (optional):
	- `.github/workflows/` – Organization-wide GitHub Actions (e.g., labeling, compliance checks, security scans).

Note: Only files in the correct paths are recognized by GitHub as globally valid. Templates and community health files in the `.github` repository apply organization-wide unless explicitly overridden in a project repository.

## Usage in Project Repositories

- Automatic inheritance: Repositories without their own templates/health files automatically use the versions stored in `.github`.
- Local overrides: Project teams can place specific templates/files in their own repo; these override the global ones.
- Referencing assets: Images/badges from `assets/` can be referenced via absolute raw links. Example: `https://raw.githubusercontent.com/Haptigation-Student-Project/.github/main/assets/<file>`.

## Maintenance, Versioning, and Release Process

- Branching: Changes are made via feature branches from `main` with a pull request.
- Review: At least one review by the maintainers of the `.github` repo is required. For policy changes (Code of Conduct, Security), two reviews are recommended.
- Versioning: Maintain simple semantic versioning at the top of files (e.g., in `CONTRIBUTING.md` as `Version: 1.2.0, Date: 2025-12-06`). Larger changes should be briefly documented in a changelog section of the respective document.
- Impact on projects: Before introducing breaking changes (e.g., PR template checklists, required fields), inform affected teams in advance (announcement in org communication channels).

## Governance and Responsibilities

- Owners: Maintainer group of the `.github` repo (organization admins or governance team). Please refer to the GitHub CODEOWNERS file in the main org repo, if available.
- Change requests: Via pull requests with clear motivation, impact assessment, and migration guidance if needed.
- Compliance: Content must comply with internal policies (security, data protection, open source policy).

## Quality Standards for Templates and Workflows

- Clarity: Short, precise checklists and instructions; avoid redundant fields.
- Accessibility: Readable language, descriptive labels; do not rely solely on color-coded hints.
- Maintainability: Centralized variables/badges, reusable action components, documented secrets/permissions.
- Security: Minimal required permissions for GitHub Actions; regularly update action versions.

## Contact, Support, and Security

- Questions/Support: Open an issue in this repository using the appropriate template.
- Security reports: Follow the instructions in `SECURITY.md` (responsible disclosure; do not open public issues for vulnerabilities).
- Emergencies: Contact the organization admins at haptigation@gmail.com.

---

Last updated: 2025-12-06
