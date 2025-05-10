# au-website
Website for Anna Mialkowska

Public URL: https://mu7trak.github.io/au-website/

Similar websites:
https://adwokatlobocka.pl/
https://smadwokaci.pl/

## Dev stuff


### Start Hugo server
``` sh
conda deactivate
conda activate au-website
# Dev deployment
cd au-website/
hugo server -D --config hugo.yaml,config-dev.yaml
```
### Hugo toha docs
https://toha-guides.netlify.app/posts/getting-started/


### Install venv
``` sh
conda create -n au-website python=3.10
conda activate au-website

pip install -r requirements.txt
```

### Get and install Hugo, GO, Node, npm
``` sh
# Get hugo
# https://themes.gohugo.io/themes/toha/

# https://discourse.gohugo.io/t/impossible-to-install-hugo-most-recent-version/45961/2
# https://github.com/gohugoio/hugo/releases/tag/v0.146.2
curl -LJO https://github.com/gohugoio/hugo/releases/download/v0.145.0/hugo_extended_0.145.0_linux-amd64.deb
sudo dpkg -i hugo_extended_0.145.0_linux-amd64.deb
rm hugo_extended_0.145.0_linux-amd64.deb
hugo version

# Get GO
# https://go.dev/dl/
wget https://go.dev/dl/go1.23.8.linux-amd64.tar.gz
sudo tar -C /usr/local -xzf go1.23.8.linux-amd64.tar.gz
go version
# Get Node 18
# https://nodejs.org/en/download/package-manager
curl -fsSL https://deb.nodesource.com/setup_18.x | sudo -E bash -
sudo apt install nodejs -y
node -v
npm -v
```

### Start Hugo template
``` sh
hugo mod init github.com/mu7trak/au-website
hugo mod tidy
```



#### Preffered files structure
``` 
your-website/
├── archetypes/
│   └── default.md  # Default archetype for content
├── assets/
│   ├── css/
│   │   └── style.scss
│   ├── js/
│   │   └── main.js
│   └── images/
│       └── logo.png
├── content/
│   ├── _index.md       # Homepage content (optional, can also be in content root)
│   ├── about/
│   │   └── index.md
│   ├── blog/
│   │   ├── my-first-post.md
│   │   └── another-post.md
│   └── projects/
│       ├── project-one.md
│       └── project-two.md
├── data/
│   └── navigation.yaml
├── layouts/
│   ├── _default/
│   │   ├── baseof.html   # Base template for all pages
│   │   ├── list.html     # Template for list pages (sections, taxonomies)
│   │   └── single.html   # Template for single content pages
│   ├── index.html        # Homepage template (overrides _default/list.html for homepage)
│   ├── partials/
│   │   ├── footer.html
│   │   └── header.html
│   └── section/          # Templates specific to content sections
│       └── blog.html
├── static/
│   ├── css/
│   │   └── extra.css   # Static CSS files
│   ├── js/
│   │   └── scripts.js  # Static JavaScript files
│   └── images/
│       └── banner.jpg  # Static images
├── themes/
│   └── your-theme/      # If using a theme
├── .gitignore
├── go.mod
├── go.sum
├── hugo.yaml
├── package.hugo.json
├── package.json
└── README.md
```


