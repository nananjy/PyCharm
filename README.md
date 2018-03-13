# PyCharm
use of PyCharm

### Tools
pycharm-**professional**-2017.3.4.exe,  
python-2.7.14.msi,  
python-3.6.4.exe.
### Draw Graph
1. Available Packages:matplotlib-**2.2.0**
2. When importing "**import matplotlib.pyplot as plt**", Error "AttributeError: module 'matplotlib' has no attribute 'verbose'", the error is as follows:  
![error verbose](https://github.com/nananjy/pyCharm/raw/master/error_verbose.png "Error verbose")
3. **Solutions**:
- Solution **one**: In PyCharm Professional 2017.3, go to **File | Settings | Tools | Python Scientific**. There is an option there to "*Show plots in toolwindow*". *Uncheck* this option. Then it should work ok.  
- Solution **two**: Try to install older version of matplotlib like 2.1.0 rather than v 2.2.0. use:  
`pip uninstall matplotlib`  
`pip install matplotlib==2.1.0`  
- Solution **three**: Change the 17th line "**verbose = matplotlib.verbose**" in the backend_interagg.py file to "**verbose = matplotlib.Verbose**".
4. Original link: [Stack Overflow](https://stackoverflow.com/questions/49146678/module-matplotlib-has-no-attribute-verbose/49158765#49158765 "module 'matplotlib' has no attribute 'verbose'").
