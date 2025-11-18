# SAM-VMNet Project Page

This repository hosts the GitHub Pages project page for the SAM-VMNet paper: **Deep Learning Model for Coronary Artery Segmentation and Quantitative Stenosis Detection**.

## Repository Structure

```
SAM-VMNet-Page/              # Project page repository
│
├── _config.yml              # Jekyll configuration (site theme, title, description)
├── index.md                 # Main project page content
├── README.md                # This file
│
├── assets/                  # Resources folder
│   ├── images/              # Paper figures and illustrations
│   │   ├── fig1_workflow.png
│   │   ├── fig4_architecture.png
│   │   ├── fig8_segmentation.png
│   │   └── fig10_stenosis.png
│   └── pdf/                 # Paper PDF files
│       └── SAM-VMNet_Paper.pdf
│
└── .gitignore               # Git ignore rules
```

## How This Page Works

This repository uses **Jekyll** with the Minimal theme to create a professional GitHub Pages project page. GitHub automatically builds and deploys this site from the main branch.

## Setup Instructions

1. Upload paper figures to `assets/images/`
2. Place the paper PDF in `assets/pdf/`
3. Customize the content in `index.md` if needed
4. Push changes to the repository

## Enabling GitHub Pages

1. Go to repository **Settings** → **Pages**
2. Under "Build and deployment", set:
   - **Source**: Deploy from a branch
   - **Branch**: main
   - **Folder**: / (root)
3. Click **Save**

The site will be available at: `https://<username>.github.io/SAM-VMNet-Page/`

## Customization

- **Theme**: Modify `theme` in `_config.yml` to change appearance (options: `jekyll-theme-minimal`, `jekyll-theme-cayman`, `jekyll-theme-slate`, etc.)
- **Content**: Edit `index.md` using Markdown
- **Styling**: Add custom CSS in `assets/css/style.css` if needed

## Related Resources

- Original Paper: [Medical Physics DOI: 10.1002/mp.17970](https://doi.org/10.1002/mp.17970)
- Code Repository: [GitHub - qimingfan10/SAM-VMNet](https://github.com/qimingfan10/SAM-VMNet)

---

**Created**: 2024  
**Purpose**: Academic project page for peer-reviewed publication
