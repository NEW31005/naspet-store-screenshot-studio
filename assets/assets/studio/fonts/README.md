# Screenshot studio font

`ipag.ttf` is the unmodified IPAGothic 00303 font, copied from Ubuntu package
`fonts-ipafont-gothic` version `00303-21ubuntu1`.

- Upstream: https://moji.or.jp/ipafont/
- Debian/Ubuntu source metadata: https://packages.ubuntu.com/fonts-ipafont-gothic
- License: `IPA_FONT_LICENSE.txt` in this directory (IPA Font License v1.0)

The screenshot-only Web build bundles this font so Japanese text never needs a
runtime font download from Google Fonts or another third-party origin.

Flutter Web also requests its Roboto regular fallback at a fixed engine path.
The unmodified official file is bundled at
`roboto/v32/KFOmCnqEu92Fr1Me4GZLCzYlKw.woff2` so this request stays same-origin.

- Source: https://fonts.gstatic.com/s/roboto/v32/KFOmCnqEu92Fr1Me4GZLCzYlKw.woff2
- SHA-256: `35b02ca266b79eb4996590f15817425a1ce9ebf48f84471843233ff614656bf2`
- License: `ROBOTO_LICENSE.txt` (Apache License 2.0)

CanvasKit requests a small set of Noto Sans CJK fallback subsets for Japanese
and CJK glyph coverage. The following unmodified Google Fonts files are kept at
the exact versioned paths requested by the engine:

- Noto Sans SC v37 `.105`: SHA-256 `a00d5f9077c22294ef7349743206eead6209feeaa40ad10313767d8d3a634e6d`
- Noto Sans SC v37 `.119`: SHA-256 `b870c13b38300611bd2aae78a2acb9da654a4eb11354fe075380753fbc7f7386`
- Noto Sans HK v32 `.118`: SHA-256 `d522f1e8a170096289a774a2e676759484efb506e9131ea10c3e77b8082614ea`
- Sources: `https://fonts.gstatic.com/s/notosanssc/v37/` and
  `https://fonts.gstatic.com/s/notosanshk/v32/`
- License: `NOTO_SANS_CJK_OFL.txt` (SIL Open Font License 1.1), copied from
  the official Google Fonts `ofl/notosanssc/OFL.txt` file. The SC and HK
  packages contain the same license text and copyright notice.
