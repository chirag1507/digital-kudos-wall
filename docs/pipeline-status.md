# Pipeline Status

This dashboard provides an overview of the component versions in different stages of the CI/CD pipeline.

## UAT Environment

**UAT Release Status:** [![Release to UAT](https://github.com/chirag1507/digital-kudos-wall/actions/workflows/release-uat.yml/badge.svg?branch=main)](https://github.com/chirag1507/digital-kudos-wall/actions/workflows/release-uat.yml)
**UAT Acceptance Tests:** [![UAT Acceptance Stage](https://github.com/chirag1507/digital-kudos-wall/actions/workflows/acceptance-stage-uat.yml/badge.svg?branch=main)](https://github.com/chirag1507/digital-kudos-wall/actions/workflows/acceptance-stage-uat.yml)

| Component | Deployed Version (on UAT)         | Last Successfully Acceptance Tested Version | Status                     |
|-----------|-----------------------------------|---------------------------------------------|----------------------------|
| Frontend  | 4b3c74a802e84c30449e414f32044677a68bde77          | 08da30cf120d2d1a91abfaad44b67f367a5a476e                       | [![Frontend Commit Stage](https://github.com/chirag1507/digital-kudos-wall-frontend/actions/workflows/commit-stage.yml/badge.svg?branch=main)](https://github.com/chirag1507/digital-kudos-wall-frontend/actions/workflows/commit-stage.yml) |
| Backend   | 5f99dc6ff99412a6f09c5d19d29c357c9787c0b9           | latest                        | [![Backend Commit Stage](https://github.com/chirag1507/digital-kudos-wall-backend/actions/workflows/commit-stage.yml/badge.svg?branch=main)](https://github.com/chirag1507/digital-kudos-wall-backend/actions/workflows/commit-stage.yml)  |

*Last updated: 2025-06-23 04:54:21 UTC*
