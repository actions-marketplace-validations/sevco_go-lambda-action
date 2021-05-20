Go AWS Lambda Builder Action
========================

![GitHub](https://img.shields.io/github/license/sevco/go-lambda-action)
![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/sevco/go-lambda-action)
![GitHub Workflow Status](https://img.shields.io/github/workflow/status/sevco/go-lambda-action/CI)
![Docker Cloud Build Status](https://img.shields.io/docker/cloud/build/sevcosec/go-lambda-action)
![Docker Image Version (latest semver)](https://img.shields.io/docker/v/sevcosec/go-lambda-action)

GitHub action for building Go based lambdas

```yaml
- uses: sevco/go-lambda-action@v1.0.0
  with:
    files: "main.go other/helper.go"
    credentials: ${{ secrets.GIT_CREDENTIALS }}
```

### Inputs
| Variable | Description | Required | Default |
|----------|-------------|----------|---------|
| files     | Source files to be built and packaged (space separated) | true | | 
| directory | Relative path under $GITHUB_WORKSPACE where source code is located | false |
| credentials | If provided git will be configured to use these credentials and https | false | |