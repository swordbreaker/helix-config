# Helix config


## Install

### Vue
```
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
```
uv tool install ty@latest
uv tool install ruff@latest
```
