# audio-data

cc [teddavis.org](https://teddavis.org) 2021

minimal tool to export peaks info from an audio file as .json
[wavesurfer.js](https://wavesurfer-js.org/) for offline analysis
created for usage with [basil.js](http://basiljs.ch)
	
### INSTALL
- download index.html, drag + drop into browser
- or, access online: [ffd8.github.io/audio-data](https://ffd8.github.io/audio-data)

### USAGE
- DRAG + DROP MP3/WAV file into browser window (or click LOAD)
- adjust SLIDER for number of peaks to output
- *optionally* [√] check 'split' to also export LEFT/RIGHT channels
- click EXPORT for .json file with info

### PARSE
- load .json with following structure:
```javascript
{
  "info": {
    "filename": "...",
    "peaksCount": 1000,
    "peaksMin": -0.4934861660003662,
    "peaksMax": 0.6202539205551147
  },
  "peaks": {
    "merged": [ ... ],
    "left": [ *if split* ],
    "right": [ *if split* ]
  }
}
```