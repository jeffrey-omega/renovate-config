# My Renovate Configuration

This repository contains my personal Renovate configuration. It is used to automatically update dependencies in my repositories.

> [!TIP]
> It is recommended to use this configuration as a base and extend it with your own settings.
> For additional information, see the [References](#references) section.

## Usage

To use this configuration, add a `.github/renovate.json` file to your repository with the following content:

```json
{
  "$schema": "https://docs.renovatebot.com/renovate-schema.json",
  "extends": ["github>jeffrey-omega/renovate-config"]
}
```

## Setup Repository Settings: (Optional)

#### Pull Requests

Recommended settings for pull requests:

- :white_check_mark: Always suggest updating pull request branches.
- :white_check_mark: Allow auto-merge .
- :white_check_mark: Automatically delete head branches.

#### Rulesets

Import the [renovate/config-validation](docs/rulesets/renovate_config-validation.json) ruleset to validate Renovate configuration changes.

## References

- [Validation of Renovate config change PRs](https://docs.renovatebot.com/config-validation/#validation-of-renovate-config-change-prs)

- [Renovate Configuration Options](https://docs.renovatebot.com/configuration-options/)

- [Config validation](https://docs.renovatebot.com/config-validation/#config-validation)

- [Renovate Presets](https://docs.renovatebot.com/presets-default/)
