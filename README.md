[![Contributors][contributors-shield]][contributors-url]
[![npm][npm-shield]](https://www.npmjs.com/package/@kontent-ai/biome-config)
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]

[![Discord][discord-shield]][discord-url]


# Kontent.ai Biome configuration

This is the Biome configuration that Kontent.ai uses for its TypeScript packages. Biome is a fast formatter, linter, and more for JavaScript, TypeScript, JSX, and JSON.

# Getting Started

1. Install the package and Biome.

    ```sh
    # Install Biome if you don't already have it
    npm i --save-dev @biomejs/biome
    # Install the shared configuration
    npm i --save-dev @kontent-ai/biome-config
    ```

2. [Extend](https://biomejs.dev/guides/configure-biome/#share-a-configuration-file) your Biome configuration by creating a `biome.json` file in your project root:

    ```jsonc
    // biome.json
    {
        "extends": ["@kontent-ai/biome-config/base"]
    }
    ```

    For React projects, you can extend the React-specific configuration:

    ```jsonc
    // biome.json
    {
        "extends": [
            "@kontent-ai/biome-config/base",
            "@kontent-ai/biome-config/react"
        ]
    }
    ```

3. Run Biome commands based on your project needs:

    ```sh
    # Format your code
    npx biome format --write .

    # Lint your code
    npx biome lint .

    # Check both formatting and linting
    npx biome check .
    ```

Available configurations are:
* `@kontent-ai/biome-config/base` (base configuration for any TypeScript/JavaScript file)
* `@kontent-ai/biome-config/react` (React specific rules, should be used together with the base configuration)

# License

Distributed under the MIT License. See [`LICENSE.md`](./LICENSE.md) for more information.


[contributors-shield]: https://img.shields.io/github/contributors/kontent-ai/biome-config.svg?style=for-the-badge
[contributors-url]: https://github.com/kontent-ai/biome-config/graphs/contributors
[npm-shield]: https://img.shields.io/badge/NPM-%23CB3837.svg?style=for-the-badge&logo=npm&logoColor=white
[forks-shield]: https://img.shields.io/github/forks/kontent-ai/biome-config.svg?style=for-the-badge
[forks-url]: https://github.com/kontent-ai/biome-config/network/members
[stars-shield]: https://img.shields.io/github/stars/kontent-ai/biome-config.svg?style=for-the-badge
[stars-url]: https://github.com/kontent-ai/biome-config/stargazers
[issues-shield]: https://img.shields.io/github/issues/kontent-ai/biome-config.svg?style=for-the-badge
[issues-url]:https://github.com/kontent-ai/biome-config/issues
[license-shield]: https://img.shields.io/github/license/kontent-ai/biome-config.svg?style=for-the-badge
[license-url]:https://github.com/kontent-ai/biome-config/blob/master/LICENSE.md
[discord-shield]: https://img.shields.io/discord/821885171984891914?color=%237289DA&label=Kontent.ai%20Discord&logo=discord&style=for-the-badge
[discord-url]: https://discord.com/invite/SKCxwPtevJ
