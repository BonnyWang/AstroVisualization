# AstroVisualization
This repo provides examples and resources for creating visualization for astro (scientific) data. 

## Particle Data
Particle data is common in astronomical simulations.

Usually, they contains the position information of particles along with related other properties (such as mass, velocity...) as the following:
| Position.x  | Position.y | Position.z | Property 1 | Property 2|
| ------------- | ------------- | ------------- | ------------- |------------- |
| ... | ... | ... |...| ... |

### Create particle visualization with Python scripting in Blender

This is suitable for people who are used to python programming experience but are overwhelmed by the thousands buttons in 3D softwares. 

#### Environment setup
1. Install Blender 
    * https://www.blender.org/
2. To use other Python library (such as pandas ) in Blender, you need to use the Python executable under the Blender folder.
    * Find the location where you install Blender. (E.g. I used the default path which is "C:\Program Files\Blender Foundation\Blender 3.6\")
    * Find the python.exe under [version_number]/python/bin
    * Right click python.exe file and select "Open in terminal"
    * In the terminal type 
        ```
        .\python.exe -m pip install [package name]
        ```
    * For example, using my path to install pandas in PowerShell would be 
        ```
        PS C:\Program Files\Blender Foundation\Blender 3.6\3.6\python\bin> .\python.exe -m pip install pandas
        ```    
#### Start creating particles in Blender
1. Open Blender and create a new "General" file
    ![alt text](Pictures\Create.png)
2. Click on the cube in the center of the view and hit delete.
3. On the top banner, select "Scripting" tab.
    ![alt text](Pictures\ScriptTab.png)
4. Click on "+ New" to create a new script.
5. Import libraries
    ```
    # This is the library for Blender
    import bpy

    # Import other library as needed
    import pandas as pd
    ```
6. The following sciprt shows an example of using a particle file to create small cubes in blender


## Other useful things to look up: 
- Blender scripting documentation
    * https://docs.blender.org/api/current/index.html
- Beginner tutorial for scripting in Blender
    * https://youtu.be/nmJqIaSZlRs?feature=shared
- Point cloud file 
    * Commonly used and supported in 3D world
- Kaze Wong's tutorial for visualizing cosmic web with Blender
    * https://github.com/kazewong/Blender_volume_tutorial
    * https://www.youtube.com/watch?v=fnbhYxj8D_s
