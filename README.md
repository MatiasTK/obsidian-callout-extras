# Callouts Extra

_Extends Obsidian [Callouts](https://help.obsidian.md/Editing+and+formatting/Callouts) functionality via a CSS Snippet_

## Features

- Card with image and text
- Card with title and text
- Card with only text
- Image aligned
- Group of cards
- Compatible with [Obsidian Style Plugin](https://github.com/mgmeyers/obsidian-style-settings)

> [!NOTE]
> Alignment can be only seen in _Reading Mode_

## Preview

### Image card with text

![card_with_text](https://i.imgur.com/vPrdT2V.png)

### Image aligned

![image_aligned](https://i.imgur.com/TSsjU28.png)

### Card with title and text

![card_with_title](https://i.imgur.com/3gqqfSp.png)

### Card with only text

![card_only_text](https://i.imgur.com/o3WwwmN.png)

### Group of cards

![group_of_cards](https://i.imgur.com/ymmWkCk.png)

## Usage

> [!IMPORTANT]
> The callout should be added before the text

### Image card with text & Card with title and text

| Identifier   | Description                                                     |
| ------------ | --------------------------------------------------------------- |
| figure       | **centered aligned** card with image or title and a description |
| figure-right | **right aligned** card with image or title and a description    |
| figure-left  | **left aligned** card with image or title and a description     |

```markdown
> [!figure] ![alt-text](link)
> Description here

> [!figure-right] ![alt-text](link)
> Description here

> [!figure-left] ![alt-text](link)
> Description here

> [!figure] Title
> Description here

> [!figure-right] Title
> Description here

> [!figure-left] Title
> Description here
```

### Image with alignment

| Identifier       | Description        |
| ---------------- | ------------------ |
| figure-img       | **centered image** |
| figure-img-right | **right aligned**  |
| figure-img-left  | **left aligned**   |

```markdown
> [!figure-img] ![alt-text](link)

> [!figure-img-right] ![alt-text](link)

> [!figure-img-left] ![alt-text](link)
```

### Cards with title

| Identifier        | Description                                       |
| ----------------- | ------------------------------------------------- |
| figure            | **centered card** with title and description      |
| figure-note-right | **right aligned card** with title and description |
| figure-note-right | **left aligned card** with title and description  |

```markdown
> [!figure]
> Description

> [!figure-note-right]
> Description

> [!figure-note-left]
> Description
```

### Cards group

| Identifier   | Description                                     |
| ------------ | ----------------------------------------------- |
| figure-group | **Group cards** in the same line, up to 3 cards |

```markdown
> [!figure-group]
>
> > [!figure] Imagen
> > Descripcion
>
> > [!figure] Imagen
> > Descripción
>
> ...
```

## Installation

1. Download `callout-extras.css` from this repo.
2. Open Obsidian and go to `Settings > Appearance`.
3. Scroll down to `Custom CSS` and click on `Open folder`.
4. Copy `callout-extras.css` into the folder.
5. Back in Obsidian, click on `Reload snippets` button.
6. Toggle the switch to enable the snippet.
7. Enjoy!

## Extra

This snippet is compatible with [obsidian-completr](https://github.com/tth05/obsidian-completr) plugin. You can use the following snippet in `.obsidian\plugins\obsidian-completr\callouts_suggestions.json` to autocomplete the callouts:

```json
{
    "displayName": "Figure",
    "replacement": "figure",
    "icon": "gallery-thumbnails",
    "color": "#ffa500"
  },
  {
    "displayName": "Figure right",
    "replacement": "figure-right",
    "icon": "gallery-thumbnails",
    "color": "#ffa500"
  },
  {
    "displayName": "Figure left",
    "replacement": "figure-left",
    "icon": "gallery-thumbnails",
    "color": "#ffa500"
  },
  {
    "displayName": "Figure image",
    "replacement": "figure-img",
    "icon": "image",
    "color": "#ffa500"
  },
  {
    "displayName": "Figure image right",
    "replacement": "figure-img-right",
    "icon": "image",
    "color": "#ffa500"
  },
  {
    "displayName": "Figure image left",
    "replacement": "figure-img-left",
    "icon": "image",
    "color": "#ffa500"
  },
  {
    "displayName": "Figure note",
    "replacement": "figure-note",
    "icon": "sticky-note",
    "color": "#ffa500"
  },
  {
    "displayName": "Figure note right",
    "replacement": "figure-note-right",
    "icon": "sticky-note",
    "color": "#ffa500"
  },
  {
    "displayName": "Figure note left",
    "replacement": "figure-note-left",
    "icon": "sticky-note",
    "color": "#ffa500"
  },
  {
    "displayName": "Figure group",
    "replacement": "figure-group",
    "icon": "layout-grid",
    "color": "#ffa500"
  }
```
