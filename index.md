---
title: "DDP9 - Demo project Sequencing report"
author: "Gaël Even"
runtime: shiny
output: ioslides_presentation
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
---


## Description of samples table

Sequencing report interpretation of a multiples samples sequencing experiments.



```
## Warning in file(file, "rt"): impossible d'ouvrir le fichier
## 'filter_step_RAW.csv' : Aucun fichier ou dossier de ce type
```

```
## Error in file(file, "rt"): impossible d'ouvrir la connexion
```

<!--html_preserve--><div id="outf0b3cb4cd9c8e4f6" class="shiny-html-output"></div><!--/html_preserve--><!--html_preserve--><div id="outec3961f71448202e" class="shiny-text-output"></div><!--/html_preserve-->



## Graphical Distribution of mean read size

<!--html_preserve--><div class="shiny-input-panel">
<div class="shiny-flow-layout">
<div>
<div class="form-group shiny-input-container">
<label class="control-label" for="bw_adjust">Bandwidth adjustment:</label>
<input class="js-range-slider" id="bw_adjust" data-min="0.2" data-max="2" data-from="1" data-step="0.2" data-grid="true" data-grid-num="9" data-grid-snap="false" data-prettify-separator="," data-keyboard="true" data-keyboard-step="11.1111111111111" data-drag-interval="true" data-data-type="number"/>
</div>
</div>
</div>
</div><!--/html_preserve--><!--html_preserve--><div id="outdf637c468cef431f" class="shiny-plot-output" style="width: 100% ; height: 400px"></div><!--/html_preserve-->

##Boxplot visualisation of number of sequences
<!--html_preserve--><div class="shiny-input-panel">
<div class="shiny-flow-layout">
<div>
<div class="form-group shiny-input-container">
<label class="control-label" for="n_breaks1">Visualize by</label>
<div>
<select id="n_breaks1"><option value="STRAIN" selected>STRAIN</option>
<option value="STATUS">STATUS</option></select>
<script type="application/json" data-for="n_breaks1" data-nonempty="">{}</script>
</div>
</div>
</div>
</div>
</div><!--/html_preserve--><!--html_preserve--><div id="out0b2bb7a2613b5819" class="shiny-plot-output" style="width: 100% ; height: 400px"></div><!--/html_preserve-->



## R summary of data

<!--html_preserve--><div class="shiny-input-panel">
<div class="shiny-flow-layout">
<div>
<div class="form-group shiny-input-container">
<label class="control-label" for="n_breaks">Column selection:</label>
<div>
<select id="n_breaks"><option value="NUMBER_SEQ" selected>NUMBER_SEQ</option>
<option value="MEAN_SIZE">MEAN_SIZE</option>
<option value="STATUS">STATUS</option>
<option value="STRAIN">STRAIN</option></select>
<script type="application/json" data-for="n_breaks" data-nonempty="">{}</script>
</div>
</div>
</div>
</div>
</div><!--/html_preserve--><!--html_preserve--><pre id="out386d0ffcf4c14829" class="shiny-text-output"></pre><!--/html_preserve-->
Conclusions :

- Homogeneous Mean read size
- Homegeneous number of sequences for humans, cows and horses
- Lower number of sequence for pigs samples
- <strong>we can play with the data!</strong>

To learn more, see [Interactive Documents](https://gdscan-gaeleven.shinyapps.io/rawcode).





