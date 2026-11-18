# Toddler Safety – Small Object Detection with Roboflow

An exploratory computer vision project investigating whether AI-powered object detection can help identify small household objects that could pose risks to toddlers.

## Project Overview

This project started with a simple parenting concern: small objects such as coins, screws, washers and toy components can easily go unnoticed around curious toddlers.

I explored this use case using [Roboflow](https://roboflow.com/), building and testing an object-detection model without having to develop a training pipeline from scratch.

## Experiment Details

| Item | Details |
|---|---|
| Platform | Roboflow |
| Task | Object Detection |
| Model | RF-DETR Small |
| Training images | 99 |
| Coin images | 67 |
| Household component and toy-part images | 32 |
| mAP@50 | 95.8% |
| Precision | 94.5% |
| Recall | 93.9% |
| F1 score | 94.2% |

## What I Explored

- Creating and preparing an object-detection dataset.
- Annotating small household objects.
- Training an object-detection model.
- Understanding validation metrics.
- Testing model predictions on additional photographs.
- Investigating missed detections and confidence thresholds.
- Identifying opportunities to improve dataset quality and model performance.

## Key Observation

Although the validation metrics were encouraging, additional testing revealed missed detections, particularly for coins at the default confidence threshold.

This highlighted the importance of testing model predictions beyond validation metrics.

## Project Article

Read the complete experiment and findings in [ARTICLE.md](ARTICLE.md).

## Limitations

This is an experimental object-detection prototype. It is not a certified choking-hazard detector or a real-time baby-monitoring system. It cannot guarantee the detection of every hazardous object or replace adult supervision.

## Future Improvements

- Expand the dataset.
- Improve class representation.
- Include more challenging real-world scenarios.
- Review annotation consistency.
- Experiment with additional image augmentations.
- Develop a more rigorous testing process.

