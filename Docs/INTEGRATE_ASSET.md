# Integrate Asset

This file is for "How to Integrate Asset Manually to your SpicaEngine Instance"

### 0. Install Spica CLI (as global)

```bash
npm i -g @spica/cli
```

### 1. Add your project to Spica context

```bash
spica context set --name <UNIQUE_NAME> --apikey <API_KEY> --url <API_URL>
```

### 2. Switch to this context

```bash
spica context switch <UNIQUE_NAME>
```

### 3. (_OPTIONAL_) Delete old asset

```bash
spica delete -f <ASSET_YAML_PATH> --ignore-not-found
```

### 4. Integrate Asset

```bash
spica apply -f <ASSET_YAML_PATH>
```
