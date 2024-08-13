## Guidelines on How to Use the Framework for Efficient Data Extraction from a Series of .sum Files

#### Motivation:

This documentation outlines the process of extracting data from a series of `.sum` files and saving the extracted data in a CSV format in a well-documented manner. At the Institut Laue-Langevin in Grenoble, France, a machine called the D20 beamline is used to perform a technique known as neutron diffraction. This technique helps us understand how neutrons bounce off the atoms in a material, specifically a material called 'oxygen transport membrane.'

The purpose of this study is to see how the structure of this material changes at different temperatures. For each specific temperature, a neutron diffraction experiment is conducted, and the resulting data is saved in a file with a ".sum" extension. Each .sum file gives us information about how the material’s structure changes at that specific temperature.

We collect a series of these .sum files at various temperatures to capture how the material’s structure evolves as the temperature changes. By converting these .sum files into CSV format, we can easily plot graphs that show how the material's structure changes with respect to temperature.

 A framework consisting of three Python scripts has been developed to achieve this task. The step-by-step workflow is described here to ensure that others can use this framework for future applications.

**Download the Scripts**:
Begin by downloading the following three Python scripts: `large_sum_step_1.ipynb`, `large_sum_step_2.ipynb`, and `large_sum_step_3.ipynb`. Save these scripts in the `User` folder on your computer. Additionally, download or copy the `.sum` files into the `User` folder. Alternatively, you may store the `.sum` files in a subfolder within the `User` folder.

**Open Jupyter Notebook**:
If Jupyter Notebook is already installed on your system, open it by searching for "Jupyter Notebook" in the Start menu. Once open, navigate to and open the file named `large_sum_step_1.ipynb`. This file will open in a new browser tab.

**Provide the Path to Your `.sum` File**

In the script, you will need to specify the path to your `.sum` file. Locate the line in the script where the file path is required. In the accompanying image, this line is highlighted within a blue rectangular box. Provide the correct path to your `.sum` file, ensuring that the path is enclosed within single quotation marks (`''`).

Once you have entered the path, click on the "Run" option, which is indicated by a pink rectangle in the image.

<img src="file:///D:/sum%20files/Picture_1.PNG" title="" alt="" data-align="center">

**Running the Second Script**

After running the first script (`large_sum_step_1.ipynb`), a set of CSV files will be generated and saved in the same directory. You can organize these files by moving them into a separate folder within the same directory.

Next, open the second script named `large_sum_step_2.ipynb`. In this script, you will need to modify two specific fields as marked in the accompanying image:

- **Blue Rectangular Box**: In this section, provide the path to the CSV files that were generated after running the first script. Ensure that the path is enclosed within single quotation marks (`''`).

- **Green Rectangular Box**: Here, specify the path where you would like to save the new set of CSV files that will be generated after running this script. Before doing so, create a new folder within the same directory to store these CSV files. Provide the full path to this new folder, again enclosed in single quotation marks (`''`).
  
  And then click "Run" option, which is indicated by a pink rectangle in the image.
  
  <img src="file:///D:/sum%20files/Picture_2.PNG" title="" alt="" data-align="center">

**Running the Final Script**

Now, open the last script named `large_sum_step_3.ipynb`. In this script, you only need to provide the path to the folder where you saved all the CSV files generated after running the second script. Ensure the path is enclosed within single quotation marks (`''`).

After entering the correct path, run the script. Once the script has finished executing, navigate to the specified folder. You will find a new CSV file named `large_sum_combined_data.csv`, which is your final desired output.

![](D:\sum%20files\Picture_3.PNG)
