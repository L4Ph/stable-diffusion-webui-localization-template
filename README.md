# stable-diffusion-webui-localization-template
## This is sd.webui-localization-template

1. Run `update-source.yaml`(GitHub Actions)
2. Pre-translated sources are generated in the `/template/source` directory.
3. Available crowdin(You need to apply to crowdin as OSS)
4. Change `lang` in lines 7,8,9 of `/tools/Merger.py` to the name of the file you want to output
5. Execute the `Merge.yaml` that has been translated(GitHub Actions)
6. `./localizations/lang.json` is output, success!