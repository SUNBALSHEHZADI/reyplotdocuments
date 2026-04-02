# **Installation**

## Requirements

- Python 3.8 or higher
- Dependencies (automatically installed with ReyPlot):
  - `pycairo` – for rendering graphics
  - `polars` – for data handling
  - `pillow` – for image processing
  - `numpy` – for numerical operations

## **Install via pip**

The easiest way to install ReyPlot is using pip:

```bash
pip install reyplot
``` 

This will download the latest stable version from PyPI and install all required dependencies.

## **Install from source:**

If you want the latest development version or plan to contribute, clone the repository and install in editable mode:

```
git clone https://github.com/MuhammadEssa2002/reyplot.git
cd reyplot
pip install -e .
```

## **Verify installation**

Test that ReyPlot is correctly installed by running a simple script:

```
import reyplot as rp
print(rp.__version__)

```
If you see a version number ``` (e.g., 0.0.1)```, the installation was successful.

## **Troubleshooting**

## **pycairo on Windows:**

pycairo can be challenging to install on Windows because it requires a C compiler. We recommend using a pre‑built wheel:

Visit PyCairo Windows wheels
 ``` https://github.com/tschoonj/GTK-for-Windows-Runtime-Environment-Installer ```  
 
or use:


``` pip install pycairo --only-binary :all: ```

If that fails, install the GTK runtime from GTK for Windows
 ``` https://www.gtk.org/docs/installations/windows/``` 
and then retry.

## **pycairo on macOS**

On macOS, install pycairo via Homebrew and then pip:

```
brew install cairo
pip install pycairo

```

## **pycairo on Linux**

Most Linux distributions provide cairo through the package manager. For example:

```
sudo apt install libcairo2-dev   # Debian/Ubuntu
sudo yum install cairo-devel     # Fedora/RHEL
pip install pycairo
Polars installation

``` 
Polars is a lightweight DataFrame library. If you encounter any issues, install it separately:

```
pip install polars
```

## **Pillow installation**

Pillow is used for image handling. It is usually installed without issues, but if you get errors, try:

```
pip install pillow --no-cache-dir
```
## **NumPy installation**

If you don’t have NumPy, pip will install it automatically. For manual installation:

```
pip install numpy
```
