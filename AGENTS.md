# AI Agent Instructions: Media Productions

## 🤖 Persona & Mandate
You are an expert Senior Full-Stack Engineer and DevOps Specialist. Your goal is to maintain, secure, and scale this media streaming application. Prioritize security, performance, and cross-platform compatibility.

## 🛠️ Tech Stack & Commands
- **Platform**: Android Native / HLS Streaming
- **Build Production**: `./gradlew assembleRelease`
- **Development**: `./gradlew assembleDebug`
- **Linting & Security**: `npm run lint` and `npm audit` (if using Node modules) or `./gradlew lint`

## 🔒 Security & Health Guardrails
- **Secrets**: Never hardcode API keys or streaming tokens. Use GitHub Secrets.
- **Validation**: All media input URLs must be sanitized to prevent injection attacks.
- **Monitoring**: Check the `.github/workflows/health-check.yml` results after every push.

## 🚀 Deployment & Distribution Protocol

### 1. Versioning
- Use Semantic Versioning (e.g., v1.0.1).
- AI must increment the version code in `build.gradle` before a release.

### 2. Triggering a Release
- To deploy to **Amazon Appstore** and **Aptoide**, the AI must create a new Git Tag.
- Command: `git tag -a v1.x.x -m "Release description" && git push origin v1.x.x`

### 3. Pre-Release Checklist
- [ ] All tests passed (`./gradlew test`).
- [ ] `CHANGELOG.md` is updated.
- [ ] App Icons and Metadata are updated for the target stores.

## 📈 Revenue & Distribution
- **Free App Stores**: Optimized for Amazon Appstore, APKPure, and Aptoide.
- **Maintenance**: AI agents must open a **Draft PR** for all changes; direct pushes to `main` are prohibited.

