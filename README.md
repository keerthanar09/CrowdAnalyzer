# CrowdAnalyzer
Microservice created to analyse crowd behaviour and patterns.

##General Pipeline

`Takes Input` (CCTV footage) -> `Divide it to zones` (16 zones) -> `Detect People using the YOLOv8 Model` -> `Extract features per zone `(such as people count, density, clustering, motion) -> `Train a classifier` (its a placeholder and will be replaced with a predictive model) -> `REturns JSON`

##CrowdAnalyser Class

*Attributes of this class include:*
- Face detection model
- Grid specifications using `gridsize`. ((4,4) suggests a 4x4 grid, creating 16 zones)
- Classifier/Predictive Model.
