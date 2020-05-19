# Zathuraconf
Create colour schemes configuration files for zathura starting from simple colour palettes provided in form of `.ini` files. To the basic configuration attributes (as indicated in `basic.conf`), we append the colour schemes by parsing the arguments given in the `.ini`.

## Installation and requirements
The script is written in Python 3.X; the only additional package needed is the command line interface `click`.  
```
git clone https://github.com/gennaro-tedesco/zathuraconf.git 
cd zathuraconf

pip install click  ## or use your favourite package manager or virtual environment
```

## Usage
Basic configuration attributes are provided in `basic.conf`: feel free to change at will. 

Colour schemes must be provided following the examples that you can find in `colour_config/*.ini`: make your own or use the default ones. Such `.ini` files must be passed as arguments to the `zathura_conf.py` script 
```
python zathura_conf.py colour_config/solarized.ini 
```
We assume the zathura configuration file that we are creating is in its standard directory `~/.config/zathura/zathurarc` as per default installation. If not, pass its location on your local machine as second command line argument to the setup script
```
python zathura_conf.py colour_config/solarized.ini ~/<new_location>/zathurarc
```

## Examples
<p align="middle">
  <img src="/examples/gruvbox.png" width="350" height="300"/>
  <img src="/examples/solarized.png" width="350" height="300"/> 
</p>
<p align="middle">
  <img src="/examples/nord.png" width="350" height="300/>
  <img src="/examples/purple.png" width="350" height="300"/> 
</p>