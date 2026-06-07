# MoSCoW Requirements

## Must Have

| ID | Requirement                                                                                                              |
| -- | ------------------------------------------------------------------------------------------------------------------------ |
| M1 | The system must detect visible rocks in raw field images using computer vision methods.                                  |
| M2 | The dataset must be reviewed and annotated before model training.                                                        |
| M3 | The project must use a consistent annotation guideline for all team members.                                             |
| M4 | The system must evaluate detection performance using suitable metrics such as precision, recall, F1 score, IoU, and mAP. |
| M5 | The project must consider lightweight models suitable for edge-device deployment.                                        |

## Should Have

| ID | Requirement                                                                                                             |
| -- | ----------------------------------------------------------------------------------------------------------------------- |
| S1 | The project should compare at least two lightweight object detection models, such as YOLO nano and YOLO small variants. |
| S2 | The project should report model size, inference time, and approximate hardware requirements.                            |
| S3 | The system should provide rough rock size categories based on bounding box area.                                        |
| S4 | The project should include qualitative error analysis using example images.                                             |

## Could Have

| ID | Requirement                                                                                                   |
| -- | ------------------------------------------------------------------------------------------------------------- |
| C1 | The system could classify rocks as fully visible or partially buried if enough reliable labels are available. |
| C2 | The project could test the model on a Raspberry Pi or similar edge device.                                    |
| C3 | The team could add extra public or self-collected ground rock images if the provided dataset is too small.    |
| C4 | The project could explore segmentation if bounding box detection is completed early.                          |

## Won’t Have for Now

| ID | Requirement                                                                                                     |
| -- | --------------------------------------------------------------------------------------------------------------- |
| W1 | The system will not estimate precise physical weight.                                                           |
| W2 | The system will not guarantee centimetre-level size estimation without a scale reference or fixed camera setup. |
| W3 | The system will not perform full autonomous rock removal.                                                       |
| W4 | The system will not treat partially buried classification as a core requirement in the first stage.             |
