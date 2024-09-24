# Callout Extras 🛠️

_Extends Obsidian [Callout](https://help.obsidian.md/Editing+and+formatting/Callouts) functionality via CSS Snippet_

## Features ⭐

- Card with image and text
- Card with title and text
- Card with only text
- Group of cards
- Image aligned
- Compatible with [Obsidian Style Settings Plugin](https://github.com/mgmeyers/obsidian-style-settings)

> [!NOTE]
> Alignment left and right can be only seen in _Reading Mode_

## Preview 🔍

You can see a [demo here](https://share.note.sx/wa0uh9g2#nxCVOJ23MuGYIOS7LTyAX51MkWmS993eNrPyXqANX2Y) or some previews in the images folder

## Installation 🚀

1. Download `callout-extras.css` from this repo.
2. Open Obsidian and go to `Settings > Appearance`.
3. Scroll down to `CSS Snippets` and click on `Open snippets folder` button.
4. Drop `callout-extras.css` into the folder.
5. Back in Obsidian, click on `Reload snippets` button.
6. Toggle the switch to enable the snippet.
7. Enjoy!

## Usage 📄

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
> Description

> [!figure-right] ![alt-text](link)
> Description

> [!figure-left] ![alt-text](link)
> Description

> [!figure] Title
> Description

> [!figure-right] Title
> Description

> [!figure-left] Title
> Description
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

### Cards without title

| Identifier        | Description                             |
| ----------------- | --------------------------------------- |
| figure-note       | **centered card** with description      |
| figure-note-right | **right aligned card** with description |
| figure-note-right | **left aligned card** with description  |

```markdown
> [!figure-note]
> Description

> [!figure-note-right]
> Description

> [!figure-note-left]
> Description
```

### Card group

| Identifier   | Description                                     |
| ------------ | ----------------------------------------------- |
| figure-group | **Group cards** in the same line, up to 3 cards |

```markdown
> [!figure-group]
>
> > [!figure] ![alt_text](link)
> > Description
>
> > [!figure] ![alt_text](link)
> > Description
>
> ...
```

## Extra 🎁

This snippet is compatible with [obsidian-completr](https://github.com/tth05/obsidian-completr) plugin. You can add the following snippet in `.obsidian\plugins\obsidian-completr\callouts_suggestions.json` to autocomplete the callout:

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
