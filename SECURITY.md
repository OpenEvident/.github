# Security Policy

## Reporting a Vulnerability

Please do not report security vulnerabilities through public GitHub issues.

Instead, use GitHub's private vulnerability reporting feature:

1. Go to the repository the vulnerability affects.
2. Open the **Security** tab.
3. Select **Report a vulnerability**.

This opens a private advisory visible only to you and the maintainers, so the issue can be discussed and fixed before any public disclosure.

If a repository does not have private reporting enabled, or you are unsure which repository is affected, open an advisory on [OpenEvident/vindicate](https://github.com/OpenEvident/vindicate/security/advisories/new) and a maintainer will redirect it if needed.

## What to include

To help us assess and reproduce the issue quickly, please include:

* A description of the vulnerability and its potential impact
* Steps to reproduce, or a proof of concept
* The affected version or commit
* Any suggested mitigation, if you have one

## What to expect

We aim to acknowledge new reports within 5 business days and to provide an initial assessment within 14 days. Timelines depend on severity and complexity; we will keep you updated as we work through it.

Once a fix is available, we will coordinate a disclosure timeline with you. We credit reporters in the advisory unless you ask to remain anonymous.

## Supported versions

OpenEvident projects are under active development. Unless a repository's own documentation states otherwise, only the latest released version receives security fixes.

## Scope

This policy covers vulnerabilities in the code maintained in OpenEvident repositories. It does not cover vulnerabilities in third party dependencies; please report those to the maintainers of the dependency directly, though we welcome a heads up so we can track and update our usage.
