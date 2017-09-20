# Black Duck CoPilot Rubygems/Codeship Basic Example

[ ![Codeship Status for BlackDuckCoPilot/example-rubygems-codeship-basic](https://app.codeship.com/projects/fc4ad9e0-6a3b-0135-a063-1e4131c2c299/status?branch=master)](https://app.codeship.com/projects/241867) [![Black Duck Security Risk](https://copilot.blackducksoftware.com/github/repos/BlackDuckCoPilot/example-rubygems-codeship-basic/branches/master/badge-risk.svg)](https://copilot.blackducksoftware.com/github/repos/BlackDuckCoPilot/example-rubygems-codeship-basic/branches/master)

Shows a working setup for using Black Duck CoPilot to analyze the risk of project dependencies

## Codeship Basic Setup
In Codeship's web interface > Project Settings > Deploy, a new deployment pipeline
has been added. The trigger is "Branch is exactly master". The "Custom Script" deployment
was chosen, and the following line added:

```sh
bash <(curl -s https://copilot.blackducksoftware.com/ci/codeshipBasic/scripts/upload)
```
