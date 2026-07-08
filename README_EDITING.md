# Editing this academic homepage

Most content can be edited without touching layout code.

## Main files

```text
_data/profile.yml        Name, title, affiliation, Google Scholar, ORCID, email
_data/research.yml       Home research categories and research-page content
_data/publications.yml   Text-only publication list
_data/cv.yml             Education, research journey, skills, awards, talks
assets/images/research/  Research images
assets/images/profile/   Profile portrait
assets/css/style.css     Visual style
```

## Replace research images

You no longer need to convert PNG to JPG. Use the same base name with any common image format:

```text
assets/images/research/01-nir-oled.png
assets/images/research/04-evaporable-fullerenes.webp
```

Supported formats: `.png`, `.jpg`, `.jpeg`, `.webp`, `.avif`, `.gif`, `.svg`.

Keep only one file with the same base name. Delete the old `.jpg` if you replace it with `.png`.

## Add a publication

Open:

```text
_data/publications.yml
```

Copy one publication block and edit the title, authors, venue, DOI, URL, year, and categories. The publication page is text-only by design.

## Update talks

Open:

```text
_data/cv.yml
```

Edit the `talks:` section. Each talk supports:

```yaml
title:
event:
location:
date:
type:
year:
```

## Upload changes

After editing files locally:

```text
GitHub Desktop -> Commit to master -> Push origin
```

## Updating publications

The publication page is controlled by:

```text
_data/publications.yml
```

Each item has these important fields:

```yaml
- sort_key: 202616
  year: 2026
  title: "Paper title"
  authors_html: "Author A, <strong>SHUI QING-JUN</strong>, Author B"
  venue: "Journal, volume, pages/article number"
  url: ""
  doi: ""
  categories: ["blue-uc-oleds"]
```

Use `sort_key` to control order. Larger numbers appear first. The website does not show citation counts; use the Google Scholar link for citation and profile updates.

