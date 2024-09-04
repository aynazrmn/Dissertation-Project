Project : Analysis of camera traps to understand activity patterns of the snow petrel (Pagodroma nivea).

The dataset consists of 266,454 images captured by ten camera traps, monitoring different nests at the Svarthamaren colony in central Dronning Maud Land, Antarctica. The cameras were set to capture images every 5 minutes and during any detected motion. Each image is embedded with metadata, including camera ID, timestamp, and temperature.

The main objectives of this project are:
1. Monitor Snow Petrel nest attendance throughout the breeding season.
2. Detect and analyze the occurrence of orange stains (from stomach oil) on Snow Petrels' bodies.
3. Assess the impact of environmental factors such as wind conditions on the activity patterns of Snow Petrels.


To achieve the objectives, the following tasks were performed:
1. Ten YOLOv8x models were trained on camera-specific datasets to detect Snow Petrels. The Computer Vision Annotation Tool (CVAT) was used to create a labeled training set, which is essential for object detection tasks to ensure accurate model training and performance.
2. Color Space Conversion for Stain Detection: Images were converted from BGR to HSV color space to isolate and detect orange stomach oil stains on the Snow Petrels. The hue range was set to 10–30, saturation to 20–255, and brightness (value) to 150–255 to capture the orange spectrum effectively. 
3. Random Forest and Gradient Boosting Models: Two models were developed to assess feature relevance between wind components (U and V) and bird activity. These models provided insights into how wind conditions influenced Snow Petrel presence in the colony.
