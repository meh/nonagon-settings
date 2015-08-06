nonagon
=======
This is a reference of bands for various instruments.

There are two settings that can be added to get the desired resut.

- `size` corresponds to the amount of samples the threshold uses before and
  after the current sample. This means the actual number of samples will be
  `size * 2 + 1`. Keep in mind all sampling is at 44100 Hz, so you don't want
  that to be too big. `25` is a good value for it, about a second worth.

- `sensitivity` is the multiplier applied the current threshold, the smaller
  the value the more sensitive it becomes. `1.5` is a magic number given by the
  gods that seems to work most of the time.

Vocals - Male
-------------
```toml
[[analyzer.beat.band]]
name  = "vocal/male:fundamental"
color = "#fff"
range = [100, 900]

[[analyzer.beat.band]]
name  = "vocal/male:harmonics"
color = "#fff"
range = [900, 8000]

[[analyzer.beat.band]]
name  = "vocal/male:high"
color = "#fff"
range = [8000, 16000]
```

Vocals - Female
---------------
```toml
[[analyzer.beat.band]]
name  = "vocal/female:fundamental"
color = "#fff"
range = [250, 900]

[[analyzer.beat.band]]
name  = "vocal/female:harmonics"
color = "#fff"
range = [1100, 8000]

[[analyzer.beat.band]]
name  = "vocal/female:high"
color = "#fff"
range = [8000, 16000]
```

Percussions - Kick
------------------
```toml
[[analyzer.beat.band]]
name  = "percussion/kick:fundamental"
color = "#fff"
range = [50, 500]

[[analyzer.beat.band]]
name  = "percussion/kick:harmonics"
color = "#fff"
range = [500, 5000]

[[analyzer.beat.band]]
name  = "percussion/kick:full"
color = "#fff"
range = [50, 5000]
```

Percussions - Tympani
---------------------
```toml
[[analyzer.beat.band]]
name  = "percussion/tympani:fundamental"
color = "#fff"
range = [60, 700]

[[analyzer.beat.band]]
name  = "percussion/tympani:harmonics"
color = "#fff"
range = [700, 3000]

[[analyzer.beat.band]]
name  = "percussion/tympani:full"
color = "#fff"
range = [60, 3000]
```
