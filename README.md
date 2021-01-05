## Geography
Repository of global and local flags and datasets with info about countries, areas, territories, regions, etc.

## Repository structure
### ./world
The folder contains flags of countries, territories, unions, and etc. In the folder you can find *info.csv* with names, population, and flag paths  
Sources: [official UN reports](https://population.un.org/wpp/Download/Standard/Population), and [wikipedia](https://en.wikipedia.org/wiki/Main_Page)
### ./american_states
The folder contains flags of the U.S. states. In the folder you can find *info.csv* with names, capitals, largest cities, population, and flag paths  
Source: [wikipedia](https://en.wikipedia.org/wiki/Flags_of_the_U.S._states_and_territories)
### ./italian_regions
The folder contains flags of italian regions. In the folder you can find *info.csv* with names, capitals, area (km.), population, and flag paths  
Source: [wikipedia](https://en.wikipedia.org/wiki/Regions_of_Italy)

## Convert SVGs to PNGs
Run the following command from a folder with images

### Linux
```bash
for file in *.svg; do inkscape $file --without-gui --export-width=1000 --export-png ${file%svg}png ; done
``` 
