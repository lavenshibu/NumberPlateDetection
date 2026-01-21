# NumberPlateDetection


## Environment

- Platform: Google Colab
- Storage: Google Drive
- Framework: Ultralytics YOLOv8

## Dependencies

- Python
- Ultralytics YOLOv8

Dependencies are installed directly inside the notebook.

## Training Pipeline

- Pretrained YOLOv8n model is used as the base model
- Custom dataset defined in `google_colab_config.yaml`
- Input image size: 640 × 640
- Training duration: 80 epochs
- Training outputs (logs, plots, weights) are generated automatically

## Model Outputs

- Outputs are stored in the `runs/` directory
- Best-performing model is saved as `best.pt`
- Results are copied to Google Drive for persistence

## Inference and Testing

- Trained model is loaded from `best.pt`
- Inference is performed on images in `test/images/`
- Confidence threshold set to 0.25
- Detection results are visualized using bounding boxes

## Tools and Libraries

- Python
- Ultralytics YOLOv8
- Google Colab
- Google Drive

## Reproducibility

To reproduce the results:

- Open `Numberplate.ipynb` in Google Colab
- Mount Google Drive
- Set the project root directory
- Install dependencies
- Run training and inference cells

## Notes

- Training and evaluation are performed in a desktop/Colab environment
- The notebook is the primary implementation
- The model can be exported for embedded deployment if required




