# ci-smoke-lab-50
Throwaway sandbox for end-to-end contribution + CI smoke test (fallback name per runbook)

## Build artifact

This repository exercises the contribution-plus-CI loop end to end. The GitHub Actions
workflow [`.github/workflows/demo.yml`](../../blob/main/.github/workflows/demo.yml)
can be triggered on demand (`workflow_dispatch`), writes a short marker file
(`demo-build.txt`), and uploads it as a build artifact named exactly **demo-build**
via `actions/upload-artifact@v4`.

artifact: demo-build
