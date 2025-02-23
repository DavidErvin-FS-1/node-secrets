# Shared Secrets

This method involves storing secrets in a separate configuration file that is included in the version-controlled repository.

## Implications:

- Security Concerns: Including secrets in the repository exposes them to anyone with access to the repository, increasing the risk of leaks.

- Collaboration Issues: Multiple developers accessing the same secrets can lead to unintentional exposures or conflicts.
