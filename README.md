# github-ado-sync-template

Template repository για αυτόματο sync GitHub → Azure DevOps.

## Περιεχόμενα

- `.github/workflows/mirror-to-ado.yml` — Sync όλων των branches και deletions από GitHub στο ADO
- `.github/workflows/build-and-publish.yml` — Build Docker image και publish στο Azure Artifacts

## Secrets που απαιτούνται

| Secret | Χρήση |
|--------|-------|
| `POC_MIRROR_SCRIPT_PAT` | ADO PAT για push στο ADO repo |
| `ADO_PUBLISH_ARTIFACT` | ADO PAT για publish στο Azure Artifacts και trigger pipeline |

## Χρήση

1. Δημιούργησε νέο repo χρησιμοποιώντας αυτό το template
2. Πρόσθεσε τα απαραίτητα secrets στο νέο repo
3. Το sync ξεκινά αυτόματα με το πρώτο push
