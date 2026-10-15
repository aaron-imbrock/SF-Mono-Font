Installation
---

```
# Create correct local fonts directory, and copy contents

mkdir -p ~/.local/share/fonts/sf-mono
cp ~/src/SF-Mono-Font/*.otf ~/.local/share/fonts/sf-mono/

# Regenerate the font cache

fc-cache -f -v

# Verify the install and the exact name

fc-list : family | grep -i "sf mono" | sort -u
```
