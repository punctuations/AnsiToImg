# Render

> Auto-generated documentation for [ansitoimg.render](../../../ansitoimg/render.py) module.

Render the ANSI

- [Ansitoimg](../README.md#ansitoimg-index) / [Modules](../MODULES.md#ansitoimg-modules) / [Ansitoimg](index.md#ansitoimg) / Render
    - [ansiToHTML](#ansitohtml)
    - [ansiToHTMLRender](#ansitohtmlrender)
    - [ansiToRender](#ansitorender)
    - [ansiToSVG](#ansitosvg)
    - [ansiToSVGRender](#ansitosvgrender)

#### Attributes

- `TEXT_HEIGHT` - monospaced chars have a constant height and width: `21`

## ansiToHTML

[[find in source code]](../../../ansitoimg/render.py#L121)

```python
def ansiToHTML(
    ansiText: str,
    fileName: str,
    theme: str | None = None,
    wide: bool = True,
):
```

Convert an ANSI stream to a html file.

#### Arguments

- `ansiText` *str* - ANSI text to convert
- `fileName` *str* - image file path
- `theme` *str, optional* - file path to base24 theme to use. Defaults to "onedark.yml".
- `wide` *bool, optional* - use a 'wide' terminal 89 vs 49 chars

## ansiToHTMLRender

[[find in source code]](../../../ansitoimg/render.py#L134)

```python
def ansiToHTMLRender(
    ansiText: str,
    fileName: str,
    theme: str | None = None,
    wide: bool = True,
):
```

Convert an ANSI stream to a Render image using pyppeteer to take a
screenshot of a generated html (hacky but we can output more like that
of a terminal now)

#### Arguments

- `ansiText` *str* - ANSI text to convert
- `fileName` *str* - image file path
- `theme` *str, optional* - file path to base24 theme to use. Defaults to "onedark.yml".
- `wide` *bool, optional* - use a 'wide' terminal 89 vs 49 chars

## ansiToRender

[[find in source code]](../../../ansitoimg/render.py#L80)

```python
def ansiToRender(
    ansiText: str,
    fileName: str,
    theme: str | None = None,
    wide: bool = True,
):
```

## ansiToSVG

[[find in source code]](../../../ansitoimg/render.py#L65)

```python
def ansiToSVG(
    ansiText: str,
    fileName: str,
    theme: str | None = None,
    wide: bool = True,
):
```

Convert an ANSI stream to SVG.

#### Arguments

- `ansiText` *str* - ANSI text to convert
- `fileName` *str* - file path to SVG to write
- `theme` *str, optional* - file path to base24 theme to use. Defaults to "onedark.yml".
- `wide` *bool, optional* - use a 'wide' terminal 89 vs 49 chars

## ansiToSVGRender

[[find in source code]](../../../ansitoimg/render.py#L84)

```python
def ansiToSVGRender(
    ansiText: str,
    fileName: str,
    theme: str | None = None,
    wide: bool = True,
):
```

Convert an ANSI stream to a Render image using pyppeteer to take a
screenshot of a generated SVG (hacky but we can get coloured emoji now)

#### Arguments

- `ansiText` *str* - ANSI text to convert
- `fileName` *str* - image file path
- `theme` *str, optional* - file path to base24 theme to use. Defaults to "onedark.yml".
- `wide` *bool, optional* - use a 'wide' terminal 89 vs 49 chars
