# DotNetApp - .NET Application

CI/CD automated deployment with GitHub Actions (Complex GitHub Flow).

## Branches
- main: Production (only receives code after successful PROD deployment)
- develop: SIT environment (automatic CI/CD)
- release/*: UAT/PROD deployments (manual approvals)
- feature/*: Feature branches for development

GitHub Flow Process:
1. feature/* branches from develop (local development)
2. PR to develop triggers CI/CD to SIT
3. Code in develop is tested in SIT
4. Create release branch for UAT/PROD
5. Manual approval for UAT deployment
6. Manual approval for PROD deployment
7. After PROD success, merge to main

