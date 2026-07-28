# Git Collaboration Sprint — Team Config

This repository contains the completed hands-on exercise from the **Revature Readiness Program** Git Collaboration Sprint. The goal of this activity was to simulate a real-world software engineering relay with a team of 5 contributors working concurrently on a shared repository.

## 🎯 Sprint Objectives
* **Pull Request Workflow:** Practice creating isolated feature branches (`feat/*`), pushing changes, opening PRs, and reviewing peer code.
* **Peer Reviews & Approvals:** Conduct line-by-line code reviews with inline feedback and formal approvals before merging.
* **Conflict Resolution Cascade:** Intentionally trigger, analyze, and manually resolve merge conflicts caused by concurrent edits to shared configuration files (`config.txt`).
* **Branch Drift & Synchronization:** Monitor branch drift (`ahead` / `behind` counts) using `git fetch` and `git status`, keeping `main` stable throughout the sprint.

## 👥 Team Roles & Responsibilities
| Role | Responsibility | Owned File |
| :--- | :--- | :--- |
| **Student A** | Repo Lead / Integrator | `README.txt` |
| **Student B** | Frontend Contributor | `src/header.txt` |
| **Student C** | Backend Contributor | `src/api-notes.txt` |
| **Student D** | Docs Contributor | `docs/setup.txt` |
| **Student E** | Reviewer / QA | `CONTRIBUTORS.txt` |

## 🔄 Sprint Execution Rounds
1. **Round 1 (Clean PRs):** Every contributor updated their designated file, submitted a PR, received a peer review, and merged cleanly into `main`.
2. **Round 2 (Conflict Cascade):** All 5 members edited `config.txt` simultaneously (bumping `BUILD_NUMBER` and adding names to `TEAM_MEMBERS`). Sequential merging required each subsequent contributor to pull `main`, resolve conflict markers (`<<<<<<<`, `=======`, `>>>>>>>`), and re-push.
3. **Round 3 (Drift & Sync):** Verified local branch drift relative to remote `main` using `git fetch`, `git log --oneline HEAD..origin/main`, and `git pull`.

---
*Completed as part of the Revature Readiness Program.*