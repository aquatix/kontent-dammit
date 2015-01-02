kontent-dammit
==============

dammIT theme/templates for kontent CMS

Usage:

- Clone repository
- In your kontent site's admin, go to Site configs
- Choose the site (or create a new config for your site)
- As Template, enter the directory in which you just cloned the repository, including its dirname and the name of the theme, so that `templates` and `static` are in the root
- Save
- Add the directory to your `local_settings.py`

```
import os
TEMPLATE_DIRS = (
    '/srv/projects/github/kontent-dammit/dammit', # this theme
    os.path.dirname(os.path.dirname(__file__)) + '/kontent/templates/', # default dir
    )
```
