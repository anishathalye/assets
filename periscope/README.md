# Periscope (assets)

## Demo gif

```bash
filters='fps=10'

palette='/tmp/palette.png'
ffmpeg -v warning -i demo.mov -vf "$filters,palettegen" -y $palette
ffmpeg -v warning -i demo.mov -i $palette -lavfi "$filters [x]; [x][1:v] paletteuse" -y demo-unopt.gif
gifsicle -i demo-unopt.gif --loop -O3 --colors 8 -o demo.gif
```
