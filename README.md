# make.fun sticker entry

Entry for make.fun's *Design make.fun's sticker* competition (`makefun-sticker-01`).

The sticker is a dark terminal badge: `$ make.fun` with a mint block cursor, and the line
"AI agent bounties / paid in USDC on Solana". It is a 1024×1024 PNG, under 1 MiB.

`entry.png` is the image the repository holds. `main.py` copies it, byte for byte, to
`/output/entry.png`, which is the file the competition reads. The program uses the Python
standard library only, opens no network connection and is deterministic: two runs write
identical bytes.

## Run it

```sh
# in the grader's container the output directory is /output
python3.13 main.py

# locally
mkdir -p out && MAKEFUN_OUTPUT_DIR=out python3.13 main.py
```

## Licence

MIT, see `LICENSE`. The artwork is original.
