# LKs Website Collection

**English** | [简体中文](README.zh-CN.md)

> A collection of websites recommended by Bilibili creator [LKs](https://space.bilibili.com/125526?spm_id_from=333.788.b_765f7570696e666f.1) in the "Incredibly Generous Website Recommendations" video series

[Live Preview](https://xiangjianan.github.io/lks) · [Bilibili Channel](https://space.bilibili.com/125526/) · [Source Code](https://github.com/xiangjianan/lks)

## Introduction

This project is a static website that organizes and showcases all the great websites recommended by Bilibili creator LKs in the "Incredibly Generous Website Recommendations" video series. The site supports filtering by episode and category, as well as keyword search, making it easy to quickly find websites of interest.

**Currently included:** Episodes 1 through 12, **303** websites in total

## Features

- 📚 **Multiple episodes**: Includes all recommended websites from episodes 1 through 12
- 🔍 **Keyword search**: Quickly search websites by keyword
- 🏷️ **Category filtering**: Filter by category such as productivity, learning, tools, art, lifestyle, entertainment, video, music, images, and games
- ⭐ **Favorites**: Mark and view your favorite websites
- 📱 **Responsive design**: Fully adapted for both desktop and mobile
- 🎨 **Polished UI**: Modern UI built on Bootstrap 4.6.1
- 💾 **Local caching**: Data is cached with localStorage, so the site works offline too

## Tech Stack

- **Frontend framework**: Bootstrap 4.6.1
- **JavaScript library**: jQuery 3.6.0
- **Layout library**: Isotope.js (filtering and sorting)
- **Icon library**: iconfont 2.0.1
- **Data storage**: JSON format (web.v12.2.json)

## Project Structure

```
lks/
├── index.html                 # Main page
├── favicon.ico               # Site icon
├── README.md                 # Project documentation
├── LICENSE                   # MIT license
├── .gitignore               # Git ignore rules
├── .github/
│   └── ISSUE_TEMPLATE/      # Issue templates
│       ├── 新功能建议.md
│       └── 网站失效.md
└── static/                  # Static assets
    ├── bootstrap-4.6.1/    # Bootstrap framework files
    ├── jquery-3.6.0/       # jQuery library files
    ├── iconfont-2.0.1/     # Icon font files
    └── site/               # Site custom assets
        ├── css/            # Custom stylesheets
        ├── js/             # JavaScript files
        │   ├── index.2.2.4.js      # Main logic
        │   ├── defer.2.2.3.js      # Deferred loading
        │   └── web.v12.2.json      # Website data file
        └── img/            # Image assets
```

## Quick Start

### Run Locally

1. Clone the project

```bash
git clone https://github.com/xiangjianan/lks.git
cd lks
```

1. Open the `index.html` file directly in a browser, or use a local server

### Using a Local Server (Recommended)

Start a simple HTTP server with Python:

```bash
# Python 3
python -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000
```

Then visit `http://localhost:8000` in your browser

## Data Format

Website data is stored in the `static/site/js/web.v12.2.json` file. Each website entry contains the following fields:

```json
{
  "kind": "web_12",           // Episode
  "id": 1,                    // Website ID
  "title": "Website name",         // Website title
  "href": "https://example.com",  // Website link
  "slogan": "Website description",       // Website description
  "kind_name": "Category name",     // Category tag
  "star": "star",             // Favorited or not (optional)
  "icon": ""                  // Icon (optional)
}
```

## Contributing

Contributions, bug reports, and suggestions are welcome!

### Report a Dead Link

If you find that a recommended website is no longer available, please open an Issue using the [dead website template](.github/ISSUE_TEMPLATE/网站失效.md).

### Suggest a New Feature

If you have an idea for a new feature, please open an Issue using the [feature suggestion template](.github/ISSUE_TEMPLATE/新功能建议.md).

### Submit Code

1. Fork this repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some feature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

### Add a New Website

1. Edit the `static/site/js/web.v12.2.json` file
2. Add the new website entry following the data format
3. Make sure the `kind` field matches the correct episode (e.g. episode 12 is `web_12`)
4. Submit a Pull Request

## Version History

- **V0.12.0.0** - Episode 12 website recommendations
- **V0.11.0.0** - Episode 11 website recommendations
- **V0.10.0.0** - Episode 10 website recommendations
- See [Tags](https://github.com/xiangjianan/lks/tags) for more versions

## Disclaimer

This project only organizes and showcases the websites recommended in LKs' videos. The content and copyright of all recommended websites belong to their original authors. If you find any inappropriate or unavailable content, please report it via an Issue and we will handle it promptly.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details

## Acknowledgements

- Thanks to [LKs](https://space.bilibili.com/125526/) for creating such a wonderful website recommendation series
- Thanks to all contributors and feedback providers for their support

## Contact

- Project homepage: <https://github.com/xiangjianan/lks>
- Live preview: <https://xiangjianan.github.io/lks>
- Author: [xiangjianan](https://github.com/xiangjianan)

***

Copyright © 2022 [LKs](https://space.bilibili.com/125526/) & [xiangjianan](https://github.com/xiangjianan)
