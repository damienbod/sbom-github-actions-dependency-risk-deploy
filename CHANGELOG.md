## ASP.NET Core, Vue.js BFF using Microsoft Entra ID Changelog

### 2026-04-21 1.1.0
- Switch SBOM generation from SPDX 3.0 to SPDX 3.1 using the Microsoft sbom-tool
- SBOM now includes `externalRef` with a VCS `locator` pointing to the GitHub repository
- Add CI validation step: workflow fails if spdxVersion ≠ SPDX-3.1 or externalRef with locator is absent
- API upload uses `SbomType: "Spdx3x"`

### 2025-12-07 1.0.0
- Updated .NET 10

### 2025-08-03 0.0.8
- Updated packages

### 2024-12-18 0.0.7
- .NET 9

### 2024-10-17 0.0.6
- Updated packages
- Updated security headers performance

### 2024-10-05 0.0.5
- Updated packages
- Updated security headers

### 2023-11-17 0.0.3
- .NET 8

### 2023-09-30 0.0.2
- Update packages
- Fixed dynamic CSP nonce injection

### 2023-09-26 0.0.1
- Initial version using Vue.js (Typescript & Vite) and ASP.NET Core
  - ASP.NET Core version 7.x
  - Vue.js (typescript & Vite)
  - CRSF used in web requests
  - Strong CSP in production
  - Azure deployment pipeline
  - Yarp proxy for development
