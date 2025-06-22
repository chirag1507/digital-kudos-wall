# Pipeline Status

This dashboard provides an overview of the component versions in different stages of the CI/CD pipeline.

## UAT Environment

**UAT Release Status:** [![Release to UAT](https://github.com/chirag1507/digital-kudos-wall/actions/workflows/release-uat.yml/badge.svg?branch=main)](https://github.com/chirag1507/digital-kudos-wall/actions/workflows/release-uat.yml)
**UAT Acceptance Tests:** [![UAT Acceptance Stage](https://github.com/chirag1507/digital-kudos-wall/actions/workflows/acceptance-stage-uat.yml/badge.svg?branch=main)](https://github.com/chirag1507/digital-kudos-wall/actions/workflows/acceptance-stage-uat.yml)

| Component | Deployed Version (on UAT)         | Last Successfully Acceptance Tested Version | Status                     |
|-----------|-----------------------------------|---------------------------------------------|----------------------------|
| Frontend  | 4396b49fc7d9fc4f1a11a023e04fd3d9cf08e51d          | 08da30cf120d2d1a91abfaad44b67f367a5a476e                       | [![Frontend Commit Stage](https://github.com/chirag1507/digital-kudos-wall-frontend/actions/workflows/commit-stage.yml/badge.svg?branch=main)](https://github.com/chirag1507/digital-kudos-wall-frontend/actions/workflows/commit-stage.yml) |
| Backend   | 5fbba536cf9e285b6c9c21792890e70e9b4c949d           | latest                        | [![Backend Commit Stage](https://github.com/chirag1507/digital-kudos-wall-backend/actions/workflows/commit-stage.yml/badge.svg?branch=main)](https://github.com/chirag1507/digital-kudos-wall-backend/actions/workflows/commit-stage.yml)  |

*Last updated: 2025-06-22 05:42:53 UTC*
