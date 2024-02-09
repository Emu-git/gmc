---
title: Muzyka
---
# Muzyka

Zengin używa [DirectMusic](https://en.m.wikipedia.org/wiki/DirectMusic) do odtwarzania ścieżki dźwiękowej w grze. Aby edytować pliki muzyczne Gothica, potrzebujesz programu [Direct Music Producer](https://en.m.wikipedia.org/wiki/DirectMusic), który został wydany przez Microsoft i był dostarczany do starszych zestawów SDK DirectX.

!!! Warning "Ostrzeżenie"
    Pliki muzyczne nie mogą być spakowane do archiwów `.vdf` lub `.mod`, wszystkie takie pliki muszą znajdować się w katalogu `/_work/Data/Music`.

## Formaty plików

Katalog `Music` zawiera następujące typy plików:

- `.dls` - Plik formatu [Downloadable Sound](https://en.wikipedia.org/wiki/DLS_format). Jest bazą dla wszystkich innych plików. Zawiera:
    - Kolekcje wirtualnych instrumentów muzycznych.
    - Pliki `.wav` używane przez instrumenty.

- `.sty` - Plik stylu. Zawiera:
    - Zespoły (Bands) - ustawienia instrumentów wirtualnych z `.dls`.
    - Wzory (Patterns) - fragmenty utworów, które można później łączyć, zapętlać i nakładać na siebie.

- `.sgt` - Plik z odpowiednio połączonymi wzorami (patternami) - końcowy utwór

## Alternatywny System Muzyczny

Plugin [zBassMusic](./union/plugins/zbassmusic.md) zastępuje domyślną bibliotekę muzyczną Zengina, dużo nowszą biblioteką BASS. Umożliwia to między innymi odtwarzanie muzyki w takich formatach jak `.mp3` lub `.ogg`, oraz pakownie utworów do archiwów `.vdf` i `.mod`.