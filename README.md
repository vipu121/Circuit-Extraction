# Circuit Extraction from Electronic Datasheets

## Description
This project uses the YOLO (You Only Look Once) model for circuit diagram extraction from electronic datasheets. The model is trained to identify and detect circuit components and symbols from images of datasheets, enabling automated processing of circuit diagrams. Additionally, the **Gemini** integration is included to extract parameters of Integrated Circuits (ICs) directly from the datasheets, providing detailed information about the components identified.

## Key Points:
- **YOLO Dataset**: The dataset used for training the model is the YOLO dataset.
- **best.pt**: The file `best.pt` contains the best-trained model parameters for the CNN (YOLO).
- **Gemini Integration**: The Gemini system is integrated to automatically extract parameters of ICs (such as Gain-Bandwidth Product, Supply Current, Input Offset Voltage, etc.) from the datasheets.
- **Testing**: The model is tested using the following datasets:
  - `ncs2`
  - `pdf2`
  - `page_119`

## How it Works:
1. **Model Training**: The YOLO model is trained on labeled images of circuit diagrams to detect and classify components.
2. **IC Parameter Extraction**: Once the circuit components are detected, Gemini extracts the relevant parameters for the ICs based on the datasheet headings and content.
3. **Testing and Results**: The model is evaluated on various test datasets to ensure accurate circuit extraction and IC parameter identification.

## Dependencies:
- YOLO (You Only Look Once)
- Gemini Integration (for IC parameter extraction)
- PyTorch
- OpenCV
- PDF Processing Libraries (e.g., pdf2image)

## How to Use:
1. Train the YOLO model using the provided dataset.
2. Integrate Gemini to automatically extract IC parameters.
3. Test the system using the sample datasets (`ncs2`, `pdf2`, `page_119`).
4. Run the model to extract circuit diagrams and IC parameters.

## Future Work:
- Expand the Gemini integration to support more IC types and parameters.
- Improve the accuracy of circuit component detection.
- Enhance the system to handle more diverse datasheets.
