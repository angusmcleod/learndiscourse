---
layout: page
lang: en
identifier: about
translations:
  -
    lang: en
    url: 'hi'
---

For the time being, the Namati Wiki is manually updated, aided by simple script utilities:

1.  Clone `https://github.com/angusmcleod/namati-wiki`
2.  Edit the `/tools/doc_list.yml` file to reflect newly added or moved pages (you can skip this step if you're only updating existing pages).
3.  Run `/tools/update_docs.rb` and `/tools/update_sidebar.rb` Ruby scripts (requires 2.1 or higher).
4.  Overwrite the top level `/_en` folder with the new folders & files in the `export` folder created by the script.
