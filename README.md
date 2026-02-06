# PantryGuard

**EU-wide Android app for household inventory management.** Track food expiry (MHD), scan barcodes, manage shopping lists, and reduce waste with smart notifications and community prices.

[![License: Apache 2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE)
[![Java 25](https://img.shields.io/badge/Java-25-orange.svg)](https://openjdk.org/)
[![Spring Boot](https://img.shields.io/badge/Spring%20Boot-4.0.2-green.svg)](https://spring.io/projects/spring-boot)
[![Android](https://img.shields.io/badge/Android-Jetpack-blue.svg)](https://developer.android.com/jetpack)

## Features (MVP)
- Barcode scanning & manual product entry
- Expiry tracking with push warnings (3/7 days)
- Shopping lists with auto-suggestions
- User auth (Google/JWT)
- Dashboard & filters

**Future:** Community prices, OCR receipts, family sharing [docs/Konzeption.md](docs/Konzeption.md)

## Architecture
Clean MVVM (Frontend) + Microservices (Backend)
- **Frontend:** Jetpack Compose/MVVM, Retrofit
- **Backend:** Spring Boot 3, PostgreSQL, Docker
- **DevOps:** Gradle, GitHub Actions, Heroku

## Quick Start
```bash
git clone https://github.com/yourusername/PantryGuard.git
cd PantryGuard
```

## Project Structure
| Folder    | Purpose                  |
| --------- | ------------------------ |
| backend/  | Spring Boot services     |
| frontend/ | Android Jetpack app      |
| shared/   | Common domain            |
| docs/     | Documentation & diagrams |
| devops/   | Deployment scripts       |

## Tech Stack
### Backend
| Component       | Technology          |
|-----------------|---------------------|
| Language        | Java 25 LTS        |
| Framework       | Spring Boot 4      |
| Database        | PostgreSQL 18      |
| ORM             | Spring Data JPA    |
| Security        | Spring Security JWT |
| Build Tool      | Gradle             |[file:1]

### Frontend
| Component      | Technology             |
|----------------|------------------------|
| Framework      | Jetpack                |
| Styling        | Material Design 3      |
| HTTP Client    | Retrofit + OkHttp      |
| State Mgmt     | ViewModel + LiveData   |
| Routing        | Navigation Component   |[file:1]

### DevOps
| Component       | Tool                  |
|-----------------|-----------------------|
| Containerization| Docker                |
| Deployment      | Heroku                |
| Orchestration   | Docker Compose        |
| Version Control | Git + GitHub          |
| CI/CD           | GitHub Actions        |[file:1]

## License
Apache 2.0 – See [LICENCSE.md](https://github.com/DukeNightshade/PantryGuard/blob/main/LICENSE) for commercial use details.
