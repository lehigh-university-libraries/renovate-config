# renovate-config

Lehigh University Library Technology's [Renovate Shareable Config Presets](https://docs.renovatebot.com/config-presets/#github)


## Usage

In the GitHub repo you want to have renovate manage updates for, add a `renovate.json5` file in the root of the repo with the contents

```
{
  $schema: 'https://docs.renovatebot.com/renovate-schema.json',
  extends: [
    'github>lehigh-university-libraries/renovate-config',
    'github>lehigh-university-libraries/renovate-config:weeklyBump.json5',
  ],
}
```

And ensure the Renovate GitHub App has your repo included in the selected repositories.
