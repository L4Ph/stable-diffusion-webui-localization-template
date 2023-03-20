# stable-diffusion-webui-localization-template
## This is sd.webui-localization-template

1. Run `update-source.yaml`(GitHub Actions)
   > Remember to set `Workflow permissions` to `Read and write permissions` in `Settings > Actions > General`.
2. Pre-translated sources are generated in the `/template/source` directory.
3. Available crowdin(You need to apply to crowdin as OSS).
4. Replace `<__lang__>` in lines 7 to 10 of `/tools/Merger.py` to the Language Codes of your language.
5. Translate on crowdin and approval pull request.
6. Execute the `Merge.yaml` that has been translated(GitHub Actions).
7. `./localizations/<__lang__>.json` is output, success!

## Directory structure will be like this:
```
📦template
 ┣📂localizations
 ┃ ┗ 📜<__lang__>.json
 ┣ 📂source
 ┃ ┣ 📂extensions
 ┃ ┃ ┣ 📂tooltips
 ┃ ┃ ┃ ┗ 📜tooltip.json
 ┃ ┃ ┗ 📜extension.json
 ┃ ┣ 📜ExtensionList.json
 ┃ ┗ 📜StableDiffusion.json
 ┗ 📂<__lang__>
   ┣ 📂extensions
   ┃ ┣ 📂tooltips
   ┃ ┃ ┗ 📜tooltip.json
   ┃ ┗ 📜extension.json
   ┣ 📜ExtensionList.json
   ┗ 📜StableDiffusion.json
```