# Algebra Compass — Raspberry Pi UI

Static Cyrillic/Latin font subsets derived from Google Fonts Comfortaa, weights 500 (Medium) and 700 (Bold). The instantiated/subset derivatives are renamed **Algebra Compass** because the original license reserves the Comfortaa name. Copyright and licensing are retained in `Comfortaa-OFL.txt` and the font name records.

Source: https://raw.githubusercontent.com/google/fonts/main/ofl/comfortaa/Comfortaa%5Bwght%5D.ttf
Source SHA-256: 0fc3f45dc48b614db9c39181502544b37217ecbf8bee2fb35886992bc96c5bd3
Retrieved 2026-11-05 over verified HTTPS. SIL Open Font License 1.1. Original source is `Comfortaa-source.ttf`; derived fonts are `AlgebraCompass-Medium.ttf` and `AlgebraCompass-Bold.ttf`.

Regenerate with `python3 scripts/build_fonts.py` (development-only fontTools dependency). Retains TrueType hinting, shaping/kerning, Cyrillic including Ё/ё, available punctuation and mathematical symbols. The script verifies the classroom alphabet, digits and operators before saving. No runtime fontTools or font download is needed. Qt uses system fallbacks for icons not covered by the family; QtAwesome has its own icon font.

The Pi DEB includes these two static files and their OFL notice. The Android companion keeps its existing typography.

---

Legacy font assets retained for source compatibility/history; not the primary Pi UI family:

# Algebra Rounded

Static Cyrillic/Latin subsets derived from Google Fonts Nunito (wght 400 / 700), renamed Algebra Rounded. Distributed under the included SIL Open Font License 1.1 (OFL.txt).

Source: https://raw.githubusercontent.com/google/fonts/main/ofl/nunito/Nunito%5Bwght%5D.ttf
Source SHA-256: bb55a5ca5c2042335b3991af27c4d0705d0ef41cac6164ac737fd8f2a1e85207
Retrieved 2026-10-30 over verified HTTPS. Source license copyright retained in OFL.txt and font name records.
Build used fontTools instancer for weights 400/700, then subset to Latin, Cyrillic, punctuation and available symbols. Renamed family, full name and PostScript name. No runtime fontTools dependency.
