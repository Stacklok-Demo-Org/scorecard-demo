[![OpenSSF Scorecard](https://api.scorecard.dev/projects/github.com/Stacklok-Demo-Org/scorecard-demo/badge)](https://scorecard.dev/viewer/?uri=github.com/Stacklok-Demo-Org/scorecard-demo)

# demo-repo-js 🦦

## Overview

The `demo-repo-js` project is a repository template primarily intended for testing and
demonstration purposes with Stacklok projects. It is a simple JavaScript project that allows you to
quickly get started with testing and demonstrating how you can use Minder and Trusty with
your JavaScript projects. It features continuous integration (CI) workflows that demonstrate how to
build, test, and sign artifacts using Sigstore and GitHub Attestations.

## Features

- Pre-configured `package.json` with `react` and `next` dependencies
- Basic tailwind CSS setup
- next.config.js with tailwind CSS support
- Dockerfile for building a container image

GitHub Actions workflows for:

- Producing signed and unsigned artifacts using Sigstore and GitHub attestations API
- Producing artifacts such as container images and binaries
- Producing container images that are reproducible (always the same digest)
- Producing "malicious" container images for testing purposes (e.g., code content was altered while building the image)

Makefile targets for simulating out-of-band signing of artifacts (both intended and not):

- Generating signed container images and "malicious" images
- Pushing container images to container registry (GHCR)
- Generating a local key pair for signing container images
- Sign container images using Sigstore by using a local key pair or by going through the Sigstore OIDC sign-in flow

Branches:

- Set of pre-created branches to use for opening PRs each demonstrating a different feature or use case with Minder and Trusty

## How to Use This Template

### GitHub Users

1. **Use this Template**:  
   Click the "Use this template" button above the file list on this repository.

2. **Create New Repository**:  
   Provide your repository with a name, description, and set the privacy settings. Click "Create repository from template."

Happy testing! 🦦🎉
