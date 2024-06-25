# OrthoDJIImage

Developer: Dr. `Haitao Lyu` (`hxl170008@utdallas.edu`)

- GitHub: [lyuhaitao (HAITAO LYU) · GitHub](https://github.com/lyuhaitao)

- LinkedIN: [https://www.linkedin.com/in/lyuhaitao](https://www.linkedin.com/in/lyuhaitao/) 

## Overview

Wild animal surveys conducted using Unmanned Aerial Vehicles (UAVs) equipped with thermal imaging cameras are a powerful tool for conservation and ecological studies. Orthogeoreferencing aligns thermal images with geographic coordinates, allowing for precise mapping of animal locations. This is crucial for spatial analysis and habitat mapping, as it provides accurate data on where animals are located within a landscape, their movement patterns, and their preferred habitats.

| ![](assets/3e4fd3c78a135be9ce04a876c65ee5e1df4f6cb4.jpg) | ![](assets/46161362d8b8d4753591465d1d90bb3f60bf732e.jpg) |
| -------------------------------------------------------- | -------------------------------------------------------- |

<img title="" src="assets/5d1a3649e53931e64e675bea02a219830c880b23.jpg" alt="" data-align="left">

Based on `PyQt6, GDAL, RasterIO, Fiona, Folium, etc`, I developed the GUI application, which can be used to  ortho-georeference thermal images captured by DJI drones.

## Download Application

Click [Download Ortho DJI Image](https://utdallas.box.com/s/m9blbm090njz2qdd57njnyyzkvt0irjz) to download the application.

Download URL: [https://utdallas.box.com/s/m9blbm090njz2qdd57njnyyzkvt0irjz](https://utdallas.box.com/s/m9blbm090njz2qdd57njnyyzkvt0irjz)

It includes a zip file, a .yml file, and a folder.

- OrthoDJIImage.zip

- buffalo. It is a folder that stores the testing thermal images captured by DJI drones.

- enviroment.yml

## Configure Running Environment

- Install `anaconda`

- Open `Anaconda prompt`

- ```conda
  conda env create -f environment.yml
  ```

- After runing the command above, a virtual environment `env_qt` will be created.

- Use the command `conda env list` to show the folder path of `env_qt`. Suppose that the path is `D:\env_qt`

- Add `D:\env_qt\Library\bin` to the system environment variable `Path`.

## Unzip OthoDJIImage.zip

![](assets/bc4fdc3258c8f5c8b49cdcfc209e8b9494253f5a.jpg)

# Getting Started

- Double click `map_view.exe`to launch the application.

![](assets/9412c26c9e851be4391184a96fd238aa8e53f704.jpg)

- Click `OpenFile` button to navigate the folder where images are stored. Double click the folder icon, then `DataView` widget will list the detailed information of each image extracted from image meta data. 

![](assets/a17b3481bf72746030d798662c4ebb8a08e12f44.jpg)

- in `DataView`, double click an item, and a new window will pop out to show the details of the corresponding image.

![](assets/e5cfe6b2ba4c8f0a4105e83874783cbd5b17455a.jpg)

- in the `DataView` widget, clicking the checkbox means that an item is selected. Click the button `Select All` to select all items. 

- Click the button `Remove`, and only the selected items are removed.

![](assets/cb34d98f74adf27902d32793d9aaa75cd2d7472f.jpg)

- Click the button `Map` . The locations where images were captured by drones will be mapped on the map in the `MapView`. 

- Locations are denoted as green icons. The arrow in a green icon represents the rotation angel of an image.

![](assets/e83e36bdf2c8cc2c2910525a93395ae621aec835.jpg)

- Click the `Layers Icon` ![](assets/6a8553d687ca1f62ae1459ffcf1b2cc188f66ec5.jpg)to pop out a new window, showing all layers. Each image is represented as a layer. 

- by selecting the checkboxes, you can decide which images will be finally chosen to stay on the map.

![](assets/99555473b4810e61b038a867114146783dbefdc8.jpg)

- Select the checkbox ![](assets/02fc20fef308e14506f282a0f0524dc08e3ed371.jpg) at the bottom, and then click the button `Map`. The frames of images will be mapped on the map.

![](assets/d5b31ad5661a0b5b94a673f0d5d5725c21836cb4.jpg)

- Click the `green icon`. A `iframe` will be pop out to show the detailed information about the image at this location.

![](assets/3aa4c321728b92c0eefb8d46c19e04b9c6f814b0.jpg)

- Click the button ![](assets/9180fcef4c798a6d68d85d03f74a999e80d1d72f.jpg). All the chosen images will be ortho-georeferenced, and saved as the `tif` files. 

- The locations and frames are written in a `ESRI shp` file.

![](assets/b0dc7625da433529b69a65d26dba43942598afd5.jpg)

![](assets/702f4665cf4cd90c762efe8bd6b1fcbf06f302ab.jpg)
