<p align="center">
  <a href="https://minnekdigital.com/">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://assets.minnekdigital.com/logo-md.jpg">
      <img alt="Minnek Logo" src="https://assets.minnekdigital.com/logo-md.jpg">
    </picture>
  </a>
</p>

---

# Big Commerce Actions

### Setup Theme Check

```yml
name: Theme Check

on:
  pull_request:
    branches: [ master ]

jobs:
  theme_check:
    uses: Minnek-Digital-Studio/bigcommerce-action/.github/workflows/theme-check.yml@master
    secrets: inherit
```

### Setup Theme Check with TypeScript

```yml
name: Theme TypeScript Check

on:
  pull_request:
    branches: [ master ]

jobs:
  theme_check:
    uses: Minnek-Digital-Studio/bigcommerce-action/.github/workflows/theme-typescript-check.yml@master
    secrets: inherit
```

### Setup Deployment

```yml
name: Deployment

on:
  pull_request:
    branches:
      - master
      - test/**

jobs:
  deployment:
    uses: Minnek-Digital-Studio/bigcommerce-action/.github/workflows/deployment.yml@master
    secrets: inherit
```

### Setup Cypress Test

```yml
name: Cypress Test

on:
  pull_request:
    branches:
      - master
      - test/**

jobs:
  cypress:
    uses: Minnek-Digital-Studio/bigcommerce-action/.github/workflows/cypress.yml@master
    secrets: inherit
```


## About

<a href="https://minnekdigital.com/">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://assets.minnekdigital.com/logo-sm.jpg">
    <img alt="Minnek Logo" src="https://assets.minnekdigital.com/logo-sm.jpg">
  </picture>
</a>

This project is maintained and funded by Minnek.

We ❤️ open source and do our part in sharing our work with the community!
See [our other projects][community] or [hire our team][hire] to help build your product.

Want to join? [Check out our Jobs][jobs]!

[community]: https://github.com/Minnek-Digital-Studio
[hire]: https://minnekdigital.com/
[jobs]: https://minnekdigital.com/careers
