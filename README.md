# sotm2018

Utilizes [Rise extension](https://github.com/damianavila/RISE) ([documentation](https://damianavila.github.io/RISE/usage.html)) to create slides from Jupyter. Just install from conda/pip to the Python kernel used by Jupyter.

## Customize

Generally most costumization options reside in the Notebook Metadata (Notebook > Edit > Edit Notebook Metadata). The current one for this project:

```json
{..,
  "livereveal": {
    "overlay": "<div class='myheader'><img class='topleft' src='../img/ors.png' alt='ors.png'><img class='topright' src='../img/uni.png' alt='ors.png'></div><div class='myfooter'><img class='lowerleft' src='../img/heigit.png' alt='heigit.png'><img class='lowerright' src='../img/kts.png' alt='kts.png'></div>",
    "theme": "simple",
    "transition": "zoom"
  },
..
}
```

The `overlay` tag can be used to customize the background slide HTML. Here, it's just setting all logos in the right place, i.e. the footer.

## Usage

To try out this notebook after `rise` installation, just run all cells first without presentation mode. Then clear all cell output (Cell > All Output > Clear).

The reason is, that many non-critical cells are skipped in the presentation and won't be executed in presentation mode.
