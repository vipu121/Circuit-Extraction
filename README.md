# YOLO Circuit Extraction from Electronic Datasheets

## Description
This project uses the YOLO (You Only Look Once) model for circuit diagram extraction from electronic datasheets. The model is trained to identify and detect circuit components and symbols from images of datasheets, enabling automated processing of circuit diagrams.

## Key Points:
- **YOLO Dataset**: The dataset used for training the model is the YOLO dataset.
- **best.pt**: The file `best.pt` contains the best-trained model parameters for the CNN (YOLO).
- **Testing**: The model is tested using the following datasets:
  - `ncs2`
  - `pdf2`
  - `page_119`
