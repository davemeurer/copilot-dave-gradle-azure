# Black Duck CoPilot Gradle/Azure Pipelines Example

[![Build Status](https://blackducksoftware.visualstudio.com/copilot-dave-gradle-azure/_apis/build/status/copilot-dave-gradle-azure-CI)](https://blackducksoftware.visualstudio.com/copilot-dave-gradle-azure/_build/latest?definitionId=9) [![Black Duck Security Risk](https://copilot.blackducksoftware.com/github/repos/BlackDuckCoPilot/copilot-dave-gradle-azure/branches/refs%2Fheads%2Fmaster/badge-risk.svg)](https://copilot.blackducksoftware.com/github/repos/BlackDuckCoPilot/copilot-dave-gradle-azure/branches/refs%2Fheads%2Fmaster)

Shows a working setup for using the Black Duck CoPilot integration to analyze the risk of project dependencies

## Azure Pipelines Setup

The `azure-pipelines.yml` file has been modified to upload generated dependency data to Black Duck CoPilot:

```yaml
- script: bash <(curl -s https://copilot.blackducksoftware.com/ci/azure/scripts/upload)
```
