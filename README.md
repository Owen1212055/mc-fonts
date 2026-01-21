# mc-fonts

Last updated: Minecraft <!--MC TOKEN-->26.1 Snapshot 4<!--MC TOKEN-->

### Information

Provides a list of all characters with their widths for each built in Minecraft font.

### Format

```json
{
  "missing_char": {
    "width": 6,
    "bold_offset": 1,
    "shadow_offset": 1
  },
  "chars": {
    "ୱ": {
      "width": 5,
      "bold_offset": 0.5,
      "shadow_offset": 0.5
    },
    "𐌾": {
      "width": 6,
      "bold_offset": 1,
      "shadow_offset": 1
    },
    "🌧": {
      "width": 9,
      "bold_offset": 1,
      "shadow_offset": 1
    }
  }
}
```

Each character is located in the ``chars`` object with each character specifying its base ``width``, ``bold_offset``, and ``shadow_offset``.
The width and bold_offset values are used to determine the position of the next char, however shadow offset does not matter and is simply used for visual purposes.

For characters that are not available in the font, minecraft will render a rectangle. This can be found under ``missing_char``.
