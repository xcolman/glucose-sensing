# Dataset from the Clinical Evaluation of a Polarization-Based Optical Noninvasive Glucose Sensing System

## Introduction
This dataset contains 962 data points from 22 participants in a clinical study using a polarization-based optical noninvasive glucose sensing system. Each participant was instructed to take measurements approximately eight times daily over a 5-day period, including measurements taken upon waking up, before and after meals, and before bedtime.The ground truth is obtained from the participants’ CGM data. This study was approved by the Institutional Review Board of Barbara Davis Center for Diabetes at University of Colorado Anschutz Medical Campus. Informed consent were obtained from all participants.

## Dataset Structure
- `data/dataset.csv`: The main dataset file.
- `data/demographic.csv`: The demographic of the participants.

## Column Descriptions
The `dataset.csv` file contains the following columns:

| Column Name               | Data Type | Description                                                              |
|---------------------------|-----------|--------------------------------------------------------------------------|
| `uid`                     | Integer   | Unique identifier for each participant.                                         |
| `pid`                     | Integer   | Unique identifier of the sensing box used.                                           |
| `ground_truth`            | Float     | The interpolated CGM value.                                                   |
| `trend_arrow`             | Integer   | The trend arrow of the CGM. <ol start="0"><li>↑↑ 2 Arrows Up</li><li>↑  1 Arrow Up</li><li>↗ Slanted Arrow Up</li><li>→ Straight Arrow</li><li>↘ Slanted Arrow Down</li><li>↓  1 Arrow Down</li><li>↓↓ 2 Arrows Down</li><li>N/A No Arrow</li></ol> |
| `{rgb}_{intensity}_{lc}`  | Float     | The raw sensor reading when a Red/Green/Blue laser diode is turned on with a specific power intensity while the liquid crystal is turned on/off. The range of the reading is 0-4095. <ul><li>rgb: r=red, g=green, b=blue</li><li>intensity: 0-99</li><li>lc: 0=off, 1=on</li></ul>|

## Citation
If you use this dataset in your research, please cite it as follows:
