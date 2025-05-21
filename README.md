# Hugo Feature Target Template

## Overview

Refer to the manual from [target-a-template](https://gohugo.io/templates/lookup-order/#target-a-template) and build a custom template for layout special request.

## Usage

```bash
git clone --single-branch -b hugo-feature-target_template https://github.com/elkan1788/hugo-travel hugo-feature-target_template
cd <branch-name>
hugo server
```

Then you can vist the page on browser with URL: [http://localhost:1313/posts/custom1/](http://localhost:1313/posts/custom1/), then found the custom layout not worked (see the post's title without Custom Layout). And the custome type [http://localhost:1313/custom/first/](http://localhost:1313/custom/first/) was woked fine. So why?

> [!WARING]
> Then you will see the `layout` paramter was not work, and the `type` paramter will work fine. On offical document suggested `type` more better, but I want to know why the `layout` not worked.