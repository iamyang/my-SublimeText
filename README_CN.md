#SublimeText相关

##下载 Sublime Text 3

[Sublime Text 3](http://www.sublimetext.com/3)

##Sublime Text Package

[Package Control](https://packagecontrol.io)

###安装 Package

输入 `ctrl+`\` 或者打开 `View > Show Console menu`. 在打开的console输入框粘贴如下代码。

Sublime Text 3:

```
import urllib.request,os,hashlib; h = 'eb2297e1a458f27d836c04bb0cbaf282' + 'd0e7a3098092775ccb37ca9d6b2e4b7d'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); by = urllib.request.urlopen( 'http://packagecontrol.io/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); print('Error validating download (got %s instead of %s), please try manual install' % (dh, h)) if dh != h else open(os.path.join( ipp, pf), 'wb' ).write(by)
```

这段代码可能会变化，如果无效，请访问[这个页面](https://packagecontrol.io/installation)。

###常用的 Package

- *[Emmet](https://packagecontrol.io/packages/Emmet)* Emmet (ex-Zen Coding) for Sublime Text.
- *[Can I Use](https://packagecontrol.io/packages/Can%20I%20Use)* Is a plugin for sublime text 2/3 for checking CSS property support.
- *[HTML-CSS-JS Prettify](https://packagecontrol.io/packages/HTML-CSS-JS%20Prettify)* HTML, CSS, JavaScript and JSON code formatter for Sublime Text 2 and 3 via node.js .
- *[Jada](https://packagecontrol.io/packages/Jade)* This was made specifically for Sublime Text 2, but was tested and works with Textmate 2 and Sublime Text 3.
- *[jQuery](https://packagecontrol.io/packages/jQuery)* Sublime Text package bundle for jQuery.
- *[Sass](https://packagecontrol.io/packages/Sass)* Sass support for TextMate & Sublime Text (2 & 3).
- *[MarkdownEditing](https://packagecontrol.io/packages/MarkdownEditing)* Powerful Markdown package for Sublime Text with better syntax understanding and good color schemes.

###移除 Package

1. `Cmd+shift+P` 输入 `rp`,找到 `Remove Package`
2. 在列表里选择你想要移除的 package
3. `Enter`


##个性化 Sublime

`Preferences -> Settings - User`

```
{
    "draw_minimap_border": true,
    "font_face": "YaHei Consolas Hybrid",
    "font_size": 17,
    "highlight_line": true,
    "ignored_packages":
    [
        "Vintage",
        "Markdown"
    ],
    "save_on_focus_lost": true
}
```

##其他

[https://github.com/jikeytang/sublime-text](https://github.com/jikeytang/sublime-text)