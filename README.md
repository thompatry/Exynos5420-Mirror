# Exynos5420 Mirror Manifest

## Using the mirror to sync

Usage: `repo init -u https://github.com/Exynos5420/mirror --mirror`

In your roomservice file, you can point to /path/to/mirror/Exynos5420/ and sync normally.

## Updating the mirror manifest

To update the mirror, use the `mirror-regen.py` script.  
Please make sure you set the environment variables before using the script:

`GHUSER` contains a valid GitHub Username and  
`GHTOKEN` contains a matching GitHub Personal Access Token  
  
To set these environment variables, run these commands in your terminal window:  

```
export GHUSER="<Your Username>"
export GHTOKEN="<Your Token>"
```

(You can obtain a GitHub Personal Access Token [here](https://github.com/settings/tokens))

**WARNING:** Please make sure no repositories have been removed before pushing a manifest change to Gerrit. A poor network connection could result in an incomplete manifest.
