# Hugo Forum Topic #54772

Details: <https://discourse.gohugo.io/t/54772>

Description: Current page properties are set incorrectly

## Instructions

Clone this branch of the repository and build the site.

```text
git clone --single-branch -b hugo-forum-topic-54772 https://github.com/elkan1788/hugo-travel hugo-forum-topic-54772
cd hugo-forum-topic-54772
hugo convert toYAML --unsafe
 cat content/_index.md
cat themes/hugo-next-v5/content/_index.md
cat themes/hugo-next-v5/content/posts/post-1.md
```

> [!NOTE]
> There used the command `hugo new theme hugo-theme-v5 --format yaml` to create new theme, but the content file's front matter still keep toml style, so sure is it a bug. Maybe it found the `content/_index.md` file is over theme's content, so not conveted it.