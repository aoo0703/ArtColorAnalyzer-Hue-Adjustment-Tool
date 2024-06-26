# ArtColorAnalyzer: Hue Adjustment Tool

ArtColorAnalyzer is a Python package that allows you to adjust the hue of images either overall or object-specifically. It leverages OpenCV, YOLOv3, NumPy, and scikit-image to provide a simple GUI for adjusting hues.

## Features

- **Overall Hue Adjustment**: Easily adjust the hue for entire images
- **Object-Specific Hue Adjustment**: With the object detection capability powered by YOLOv3, you can selectively adjust the hue of specific objects within an image. For instance, in scenes containing multiple elements like people, cars, and trees, you can modify the hue of just the car while leaving the other elements unaffected. Additionally, you can adjust the hue within selected grids. This feature proves beneficial for complex images where object detection is challenging, such as paintings or abstract art.

- See example.py if you want to try it too!

### Example of Object-Specific Hue Adjustment
Object-Specific Hue Adjustment (Cup):
![Adjusted Image](adjusted_image/object_adjusted_image.png)

### Example of Grid-Based -- Object-Specific Hue Adjustment
Grid-Based -- Object-Specific Hue Adjustment:
![Adjusted Image](adjusted_image/grid_adjusted_image.png)

## file structure
```sh
artcoloranalyzer/
├── artcoloranalyzer/
│   ├── __init__.py
│   ├── analyzer.py
│   ├── overall_hue_adjustment.py
│   ├── object_specific_hue_adjustment.py
│   └── yolov3/
│       ├── yolov3.cfg
│       ├── yolov3.weights
│       └── coco.names
├── example_image/
│   ├── 00_kaiga.JPG
│   ├── breakfast.png
├── example.py
├── README.md
├── YOLOv3_LICENSE
└── LICENSE
```

- please Download ```yolov3.weights``` and place it under yolov3 as in the structure above

...

## Third-Party Licenses

This project includes code and data from the YOLOv3 project. The YOLOv3 project is licensed under the Apache License 2.0. For more information, see the `YOLOv3_LICENSE` file included in this repository.

...

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

The YOLOv3 components are licensed under their respective licenses - see the [YOLOv3_LICENSE](YOLOv3_LICENSE) file for details.


## Installation

You can install the package via pip:

```sh
pip install ArtColorAnalyzer
