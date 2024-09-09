# Academic Kickstart

---

This code is used to create the Zippel Lab website: https://zippelsf.github.io/

## How to update
- Update content in the /content directory, or one of the /config files
- add, commit, and push changes to this repository (i.e., https://github.com/zippelsf/academic-kickstart)
- cd to the website directory in a terminal and use the command: `hugo`
- cd to the /public folder, add, commit, and push changes
- the website should update in a few minutes after changes are pushed
- see documentation here for more (https://wowchemy.com/docs/guide/deployment/)

## Add a publication
- We are using: https://github.com/wowchemy/hugo-academic-cli (also see https://wowchemy.com/docs/content/publications/)
- install academic with pip3
- use the command:  `academic import --bibtex ./static/pubs/publist.bib`
- (Hint: make sure academic is in your path - issues after OS updates)

## Troubleshooting
- Issues with making a local hugo server, with error: `failed to extract shortcode: template for shortcode "alert" not found` try clearing the cache with:
```
hugo mod clean
hugo mod get -u ./...
```