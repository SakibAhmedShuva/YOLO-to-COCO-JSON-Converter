# YOLO-to-COCO-JSON-Converter

A robust Python tool for converting YOLO format annotations to COCO JSON format, with additional support for duplicate file detection.

## Note: Your images folder must not contain any image with same name but different extensions like:
cars_0001.jpg

cars_0001.jpeg

Use deduplicator.ipynb to find and remove such duplicated files.

## Features

- Convert YOLO annotations to COCO JSON format
- Support for both bounding box and segmentation annotations
- Handles train/val/test splits automatically
- Duplicate file detection and reporting
- Progress tracking during conversion
- Maintains unique image IDs even with duplicate filenames

## Installation

```bash
git clone https://github.com/SakibAhmedShuva/YOLO-to-COCO-JSON-Converter.git
cd YOLO-to-COCO-JSON-Converter
open yolo2coco.ipynb
```

## Directory Structure

Your YOLO dataset should be structured as follows:

```
dataset/
├── data.yaml
├── train/
│   ├── images/
│   └── labels/
├── val/
│   ├── images/
│   └── labels/
└── test/
    ├── images/
    └── labels/
```

## data.yaml Format

```yaml
train: ../train/images
val: ../valid/images
test: ../test/images

names:
  0: class1
  1: class2
  ...
```

## Screenshot
## Output:
![{2B084F2B-EE21-45C6-B1C9-EEB0ED296A7A}](https://github.com/user-attachments/assets/e425a620-b3af-4662-8da9-e6dc75a993d6)


## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Thanks to all contributors who have helped with the development of this tool
- Inspired by the need for reliable YOLO to COCO conversion in computer vision projects
