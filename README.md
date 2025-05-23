# Hugo Feature Merge

## Overview

Refer the offical document from [configuration-merge](https://gohugo.io/configuration/introduction), to learn the configuration merge rules. And found that had 3 rule with different paramaters, so  when you design the `hugo.yaml` config file template, need to unstand whether parameter's merge is none. If it's true, then you need add the custom merge rule in site's `hugo.yaml`, kind the like as below:

```yaml
markup:
  _merge: deep

minify:
  minifyOutput: true

enableEmoji: true
enableRobotsTXT: true
```

## Usage

```bash
git clone --single-branch -b hugo-feature-merge_config https://github.com/elkan1788/hugo-travel hugo-feature-merge_config
cd hugo-feature-merge_config
hugo server
```

> [!NOTE]
> Then visit the default URL [http://localhost:1313/](http://localhost:1313/) on browser, you will find that site's configuration will override the theme's configuration.