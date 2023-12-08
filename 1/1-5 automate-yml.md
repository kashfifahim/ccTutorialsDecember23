# Structure of CrossCompute's Automate.yml Config File
When working with the CrossCompute Framework you are going to be primarily customizing the configuration file called ```automate.yml```.  In this article let us explore the structure of this config file and some of its commonly used settings and parameters for automated processes or applications. 

The ```automate.yml``` file is divided into several key sections, each serving a distinct purpose. Let's break down these sections and explore the various views available for use.

### Header Section
- crosscompute: Specifies the version of the CrossCompute tool being used.
- name: Provides a name for the setup, in this case, "Test Variable Views".
- version: Indicates the version of this particular configuration.

### Input Section
This section defines the inputs required by the application. Each input variable has an id, view, path, and additional attributes like label and configuration.
- variables: A list of different variables required as input, each having unique properties.
  - view: Specifies the type of input, like string, number, password, etc.
  - path: Indicates where the input data is stored or the source path.

### Output Section
This section is similar to the input section but defines the output variables of the application.
- Each output variable includes a view, path, and sometimes configuration and mode.
- view: Different types like link, string, number, image, etc., are used to define how the output will be presented.
- templates: Specifies markdown templates for output data.

### Batches Section
Defines batch processing folders.

### Display Section
The display section specifies CSS styles and page configurations for the automation interface.
- styles: Links to CSS stylesheets.
- pages: Defines different pages of the automation interface, each with its own design configuration.

## Variety of Views
The automate.yml file supports a diverse range of views for both input and output variables. These views define how the data is presented or captured in the user interface. Some of the views include:

- Textual Views: string, number, text, markdown, and password. These are used for capturing or displaying basic text, numbers, or formatted text content.
- File Views: file, image, pdf, json, and table. These views handle file inputs and outputs, ranging from simple file uploads to displaying images and tables.
- Interactive Views: radio, checkbox, and frame. Used for interactive elements like radio buttons, checkboxes, or embedded frames.
- Map Views: map-mapbox-location, map-mapbox, and map-deck-screengrid. These are specialized views for geographical data representation using maps.

![A demo of the different input views available to use for your automation](./images/DifferentViews.png)

In conclusion, the automate.yml file is a versatile configuration tool that allows for detailed customization of input and output variables, with a wide range of view options to cater to different data types and user interface requirements. Learning and understanding the structure and options available in this file will enhance the effectiveness and user-friendliness of your automated processes or applications.