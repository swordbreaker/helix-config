# Helix config

See also [Helix Language Servers](https://helix-editor.vercel.app/reference/language-servers)

## Install

### Vue
```sh
bun add -g @tailwindcss/language-server typescript typescript-language-server @vue/typescript-plugin vscode-langservers-extracted @biomejs/biome
```

### biome configuration for vue:
```json
{
    "$schema": "./node_modules/@biomejs/biome/configuration_schema.json",
    "html": {
        "experimentalFullSupportEnabled": true,
        "formatter": {
            "indentScriptAndStyle": false
        }
    },
    "overrides": [
        {
            "includes": ["**/*.vue"],
            "formatter": {
                "enabled": true,
                "formatWithErrors": true
            }

          },
    ],
}
```json

### Python
```sh
uv tool install ty@latest
uv tool install ruff@latest
```

### Dependecy Managment
```sh
cargo install deps-lsp
```

### Others
```sh
# Bash
bun add -g bash-language-server
# Docker
bun add -g dockerfile-language-server-nodejs
# Docker Compose
bun add -g @microsoft/compose-language-service
# Yaml
bun add -g yaml-language-server@next

# English grammar and spelling checker
cargo install harper-ls --locked

# TOML formatting
cargo install taplo-cli --locked
```
