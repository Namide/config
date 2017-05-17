# Config Sublime Text 3

## Install Package Control

```python
import urllib.request,os,hashlib; h = 'df21e130d211cfc94d9b0905775a7c0f' + '1e3d39e33b79698005270310898eea76'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); by = urllib.request.urlopen( 'http://packagecontrol.io/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); print('Error validating download (got %s instead of %s), please try manual install' % (dh, h)) if dh != h else open(os.path.join( ipp, pf), 'wb' ).write(by) 
```

> To add some plugin use the command `Package Control: Install Package`


## Plugins

- Emmet
- CSS Extended Completions  
- DocBlockr

- SublimeLinter
- TernJS

- Material Theme
- MarkdownHighlighting
- OpenGL Shading Language (GLSL)

- Open Folder
- Terminal


## Settings

```js
{
    "auto_complete_triggers":
    [
        {
            "characters": "<",
            "selector": "text.html"
        },
        {
            "characters": ".",
            "selector": "source.js"
        }
    ],
    "color_scheme": "Packages/Material Theme/schemes/Material-Theme.tmTheme",
    "font_size": 14,
    "ignored_packages":
    [
        "Vintage"
    ],
    "material_theme_accent_acid-lime": true,
    "material_theme_accent_scrollbars": true,
    "material_theme_arrow_folders": true,
    "material_theme_compact_panel": true,
    "material_theme_compact_sidebar": true,
    "material_theme_contrast_mode": true,
    "material_theme_disable_fileicons": true,
    "material_theme_small_tab": true,
    "material_theme_tabs_autowidth": true,
    "material_theme_tabs_separator": true,
    "rulers":
    [
        80
    ],
    "tab_size": 4,
    "theme": "Material-Theme.sublime-theme",
    "translate_tabs_to_spaces": true,
    "word_wrap": true,
    "wrap_width": 80
}
```