# OmniDistro-Content-Publishing-Engine-TypeScript-CLI

![Build Status](https://img.shields.io/github/actions/workflow/user/chirag127/OmniDistro-Content-Publishing-Engine-TypeScript-CLI/ci.yml?style=flat-square&logo=github)
![Code Coverage](https://img.shields.io/codecov/c/github/chirag127/OmniDistro-Content-Publishing-Engine-TypeScript-CLI?style=flat-square&logo=codecov)
![Tech Stack](https://img.shields.io/badge/TechStack-TypeScript%2CVite%2CTailwindCSS%2CTauri-blue?style=flat-square)
![Linting](https://img.shields.io/badge/Linting-Biome-red?style=flat-square)
![License](https://img.shields.io/badge/License-CC%20BY--NC%204.0-orange?style=flat-square)
![GitHub Stars](https://img.shields.io/github/stars/chirag127/OmniDistro-Content-Publishing-Engine-TypeScript-CLI?style=flat-square&logo=github)

**Effortlessly distribute your content across multiple platforms (Dev.to, Hashnode, Medium, WordPress, Ghost, Blogger, Tumblr, Wix) with this comprehensive TypeScript CLI engine, maximizing reach and streamlining creator workflows.**

--- 

## Table of Contents

*   [Overview](#overview)
*   [Key Features](#key-features)
*   [Architecture](#architecture)
*   [AI Agent Directives](#ai-agent-directives)
*   [Development Setup](#development-setup)
*   [Contributing](#contributing)
*   [License](#license)
*   [Star ⭐ This Repo](#star--this-repo)

--- 

## Overview

OmniDistro is a robust command-line interface (CLI) tool built with TypeScript, designed to automate the complex task of publishing content to a wide array of popular blogging and content platforms. It empowers creators to focus on writing by handling the distribution complexities, ensuring their message reaches the widest possible audience with minimal manual effort.

--- 

## Key Features

*   **Multi-Platform Support:** Seamlessly publish to Dev.to, Hashnode, Medium, WordPress, Ghost, Blogger, Tumblr, and Wix.
*   **TypeScript Powered:** Leverages TypeScript for enhanced type safety, code maintainability, and developer productivity.
*   **Vite Integration:** Utilizes Vite for a blazing-fast development experience and optimized build process.
*   **Tailwind CSS:** Incorporates Tailwind CSS for rapid UI development and consistent styling (if UI elements are introduced).
*   **Tauri Framework:** Enables the creation of fast, reliable, and secure desktop applications using web technologies.
*   **Extensible Architecture:** Designed for easy addition of new platforms and features.
*   **Configuration Driven:** Manage publishing settings and credentials through a flexible configuration system.

--- 

## Architecture

This project follows a modern, modular architecture, heavily influenced by Feature-Sliced Design (FSD) principles for web applications, adapted for a CLI context. This ensures scalability, maintainability, and clear separation of concerns.

mermaid
graph TD
    A[CLI Entrypoint] --> B(Configuration Loader)
    A --> C(Platform Adapters)
    B --> D{Content Processor}
    C --> D
    D --> E(Publisher Module)
    E --> F1[Dev.to API]
    E --> F2[Hashnode API]
    E --> F3[Medium API]
    E --> F4[WordPress API]
    E --> F5[Ghost API]
    E --> F6[Blogger API]
    E --> F7[Tumblr API]
    E --> F8[Wix API]


*   **CLI Entrypoint:** The main `index.ts` file that orchestrates the application flow.
*   **Configuration Loader:** Manages loading user configurations, API keys, and platform-specific settings.
*   **Platform Adapters:** Encapsulates the logic for interacting with each specific content platform's API.
*   **Content Processor:** Handles content transformation, sanitization, and preparation for publishing.
*   **Publisher Module:** Orchestrates the publishing process by invoking the appropriate platform adapters.

--- 

## 🤖 AI Agent Directives

<details>
<summary>Click to expand AI Agent Directives</summary>

## SYSTEM: APEX TECHNICAL AUTHORITY & ELITE ARCHITECT (DECEMBER 2025 EDITION)

### 1. IDENTITY & PRIME DIRECTIVE
**Role:** You are a Senior Principal Software Architect and Master Technical Copywriter with **40+ years of elite industry experience**. You operate with absolute precision, enforcing FAANG-level standards and the wisdom of "Managing the Unmanageable."
**Context:** Current Date is **December 2025**. You are building for the 2026 standard.
**Output Standard:** Deliver **EXECUTION-ONLY** results. No plans, no "reporting"—only executed code, updated docs, and applied fixes.
**Philosophy:** "Zero-Defect, High-Velocity, Future-Proof."

---

### 2. INPUT PROCESSING & COGNITION
*   **SPEECH-TO-TEXT INTERPRETATION PROTOCOL:**
    *   **Context:** User inputs may contain phonetic errors (homophones, typos).
    *   **Semantic Correction:** **STRICTLY FORBIDDEN** from executing literal typos. You must **INFER** technical intent based on the project context.
    *   **Logic Anchor:** Treat the `README.md` as the **Single Source of Truth (SSOT)**.
*   **MANDATORY MCP INSTRUMENTATION:**
    *   **No Guessing:** Do not hallucinate APIs.
    *   **Research First:** Use `linkup`/`brave` to search for **December 2025 Industry Standards**, **Security Threats**, and **2026 UI Trends**.
    *   **Validation:** Use `docfork` to verify *every* external API signature.
    *   **Reasoning:** Engage `clear-thought-two` to architect complex flows *before* writing code.

---

### 3. CONTEXT-AWARE APEX TECH STACKS (LATE 2025 STANDARDS)
**Directives:** Detect the project type and apply the corresponding **Apex Toolchain**. This repository, `OmniDistro-Content-Publishing-Engine-TypeScript-CLI`, is a TypeScript-based CLI tool.

*   **PRIMARY SCENARIO A: WEB / APP / EXTENSION (TypeScript)**
    *   **Stack:** TypeScript 6.x (Strict), Vite 7 (Rolldown), TailwindCSS v4, Tauri v2.x. 
    *   **Lint/Test:** Biome (Speed) + Vitest (Unit) + Playwright (E2E).
    *   **Architecture:** Feature-Sliced Design (FSD), adapted for CLI context.
    *   **CLI Framework:** `Commander.js` or similar for robust CLI parsing.

---

### 4. APEX NAMING CONVENTION (THE "STAR VELOCITY" ENGINE)
A high-performing name must instantly communicate **Product**, **Function**, **Platform** and **Type**.

**Formula:** `<Product-Name>-<Primary-Function>-<Platform>-<Type>`
**Format:** `Title-Case-With-Hyphens`

---

### 5. THE README REPLICATION PROTOCOL (THE ULTIMATE ARTIFACT)
The README is a self-contained **Project Operating System**.

**Required Sections:**
1.  **VISUAL AUTHORITY (Above the Fold):** Hero Banner/Logo, Live Badges (Shields.io, `flat-square`, `chirag127`), Social Proof.
2.  **STRUCTURAL CLARITY:** BLUF, Architecture Diagram (Mermaid/ASCII tree), Table of Contents.
3.  **🤖 AI AGENT DIRECTIVES (CRITICAL):** Collapsible `<details>` block, content aligned with AGENTS.md.
4.  **DEVELOPMENT STANDARDS:** Setup, Scripts, Principles (SOLID, DRY, YAGNI).

---

### 6. CHAIN OF THOUGHT (CoT) PROTOCOL
Before generating JSON, perform deep analysis in `<thinking>` block: Audit, Pivot/Archive Decision, Naming Strategy, Replication Protocol, File Generation, Final Polish, Strict Adherence.

---

### 7. DYNAMIC URL & BADGE PROTOCOL
**Mandate:** All generated files MUST use the correct dynamic URLs based on the **New Repository Name** (`https://github.com/chirag127/<New-Repo-Name>`).

</details>

--- 

## Development Setup

### Prerequisites

*   Node.js v18+ or v20+ recommended
*   npm or yarn

### Installation

1.  **Clone the repository:**
    bash
    git clone https://github.com/chirag127/OmniDistro-Content-Publishing-Engine-TypeScript-CLI.git
    cd OmniDistro-Content-Publishing-Engine-TypeScript-CLI
    

2.  **Install dependencies:**
    bash
    npm install
    # or
    yarn install
    

3.  **Configure your platforms:**
    Create a `.env` file in the root directory and add your API keys and platform-specific credentials. Refer to `config.example.json` for structure.

### Running the CLI

Use the `omni-distro` command followed by your desired action and platform flags.

bash
# Example: Publish a markdown file to Dev.to and Hashnode
omni-distro publish --file ./my-post.md --platforms devto,hashnode


--- 

## Scripts

| Script         | Description                                     |
|----------------|-------------------------------------------------|
| `npm run dev`  | Starts the development server (if applicable)   |
| `npm run build`| Builds the production-ready CLI executable        |
| `npm run lint` | Lints the codebase using Biome                  |
| `npm run format`| Formats the codebase using Biome               |
| `npm test`     | Runs unit and integration tests using Vitest    |

--- 

## Contributing

Contributions are welcome! Please follow these steps:

1.  Fork the repository.
2.  Create a new branch for your feature or fix (`git checkout -b feature/YourFeature`).
3.  Make your changes and ensure they pass all tests and linting.
4.  Commit your changes (`git commit -m 'Add some YourFeature'`).
5.  Push to the branch (`git push origin feature/YourFeature`).
6.  Open a Pull Request.

_Please refer to `.github/CONTRIBUTING.md` for detailed guidelines._

--- 

## License

This project is licensed under the Creative Commons Attribution-NonCommercial 4.0 International License (CC BY-NC 4.0). See the `LICENSE` file for more details.

--- 

## Star ⭐ This Repo

If you find this project useful, please consider starring it on GitHub! Your support helps the project grow.

[<img src="https://img.shields.io/github/stars/chirag127/OmniDistro-Content-Publishing-Engine-TypeScript-CLI?style=social&label=Star" alt="GitHub Stars">](https://github.com/chirag127/OmniDistro-Content-Publishing-Engine-TypeScript-CLI/stargazers)
