# Smaller Gallery :mount_fuji:

Copies everything and resizes the pictures for a more usable viewing UX.

## Notes

- Resizes `.png`, `.jpg`, `.jpeg` extensions (case-insensitive).
- Is recursive
- Copies/Resizes only non-existing files to save time
- Uses simple Bash scripting

## Configuration

| Argument | Default | Description |
|---|---|---|
| `-w`, `--width` | `1000` | width of pictures |
| `-i`, `--in` | `./original/` | dir of original files |
| `-o`, `--out` | `./gallery/` | dir of gallery with smaller images |

## Example

```
./bin/smallergallery -v && \
./bin/smallergallery --in ./example/original/ --out ./example/gallery/ --width 600
```

## Dependencies

Run `smallergallery -v` to test.

- convert
- find
- pushd
- realpath
- mkdir
- read
- dirname
- rsync
- bash

## License

[MIT](/LICENSE)
