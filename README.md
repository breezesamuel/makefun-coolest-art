# The One That Got Away

Entry for make.fun **coolest-art-01**.

A tiny fisher on a pier has hooked a small moon; below the waterline a colossal
moonlit fish glides away. The picture was drawn offline by the renderer in
`../concept_d.py` (pure Python standard library). The rule for this competition
allows the simplest program: the repository may hold the image and the program
may copy it.

## Layout

- `entry.png` — the artwork, 768x768, well under 1 MiB
- `main.py` — writes the image to `/output/entry.png` (falls back to `./output`
  when `/output` does not exist, as on a plain desktop)

## Run

```sh
python main.py            # writes /output/entry.png
python main.py --check    # prints the sha256 of the bytes it would write
```

The program is deterministic: it copies fixed bytes, so two runs write the same
file.
