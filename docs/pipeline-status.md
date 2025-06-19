# Pipeline Status

This dashboard provides an overview of the component versions in different stages of the CI/CD pipeline.

## UAT Environment

**UAT Release Status:** [![Release to UAT](https://github.com/chirag1507/digital-kudos-wall/actions/workflows/release-uat.yml/badge.svg?branch=main)](https://github.com/chirag1507/digital-kudos-wall/actions/workflows/release-uat.yml)
**UAT Acceptance Tests:** [![UAT Acceptance Stage](https://github.com/chirag1507/digital-kudos-wall/actions/workflows/acceptance-stage-uat.yml/badge.svg?branch=main)](https://github.com/chirag1507/digital-kudos-wall/actions/workflows/acceptance-stage-uat.yml)

| Component | Deployed Version (on UAT)         | Last Successfully Acceptance Tested Version | Status                     |
|-----------|-----------------------------------|---------------------------------------------|----------------------------|
| Frontend  | 81bd7015c96cafdca07e8ccac065e3af9099e17d          | 08da30cf120d2d1a91abfaad44b67f367a5a476e                       | [![Frontend Commit Stage](https://github.com/chirag1507/digital-kudos-wall-frontend/actions/workflows/commit-stage.yml/badge.svg?branch=main)](https://github.com/chirag1507/digital-kudos-wall-frontend/actions/workflows/commit-stage.yml) |
| Backend   | 48083e376b6618de8d4a5404e08c697db57299c5           | latest                        | [![Backend Commit Stage](https://github.com/chirag1507/digital-kudos-wall-backend/actions/workflows/commit-stage.yml/badge.svg?branch=main)](https://github.com/chirag1507/digital-kudos-wall-backend/actions/workflows/commit-stage.yml)  |

*Last updated: 2025-06-19 11:39:22 UTC*
