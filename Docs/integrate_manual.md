# Integrate Asset manually

This file is for "How to Integrate Asset Manually to your SpicaEngine Server or Instance?".

### **0. Install Spica CLI (as globally)**

```bash
npm i -g @spica/cli
```

### **1. Add your project to Spica context**

```bash
spica context set --name <UNIQUE_NAME> --apikey <API_KEY> --url <API_URL>
```

### **2. Switch to this context**

```bash
spica context switch <UNIQUE_NAME>
```

### **3. (_OPTIONAL_) Delete old asset**

```bash
spica delete -f <ASSET_YAML_PATH> --ignore-not-found
```

### **4. Integrate Asset**

```bash
spica apply -f <ASSET_YAML_PATH>
```

> **Congratulations, Asset successfully integrated.**

---

## Terminology

```
<UNIQUE_NAME>   |It should be a unique name for the spica server on your computer. You can name whatever you want.
```

```
<API_KEY>   |API key from your server. It should have "Strategy Full Access" in policies.
```

```
<API_URL>   |API url of your server. Generally "https://server_url.com/api".
```

```
<ASSET_YAML_PATH>   |Path of the asset's yaml file. If in the same file with .yaml just type yaml_name.yaml.
```

```
--ignore-not-found  |This option will ignore the error messages if it will not find the related asset.
```
