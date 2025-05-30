# Disqus Plugin for Minniark

The Disqus plugin adds a comment section below blog posts using the [Disqus](https://disqus.com/) platform. It can be enabled globally and configured via a settings.json file, while individual posts can toggle comment visibility using a custom field.

Features:
* Seamless integration of Disqus comment threads
* Global enable/disable setting via settings.json
* Per-post control via a post.yml toggle field
* Automatically available in Twig templates via {{ plugin.disqus.html|raw }}
Requirements:
* A Disqus account with a registered shortname
* a aktive minniark installation

## Installation

Upload the `disqus` folder into the `/userdata/plugins` dir and enable it in the plugin dashboard.

## Usage

To use the plugin in your post.twig file, you need only the following lines of code.
```
{% if plugin.disqus.enabled %}                    
  {{ plugin.disqus.html|raw }}
{% endif %}
```

© 2025 [Christian Heinisch](https://heimfisch.de)  
Released under the [MIT license](https:/minniark.app/license)
