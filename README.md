# Calculator automat de scor pentru jocul Mathable folosind Computer Vision

## Description
This project implements an automated score calculator for the Mathable board game using computer vision techniques. The system processes images of the game board, detects the played tiles, and calculates the score based on the game rules.


## Features

### Board Detection & Processing
- HSV color space conversion for robust board detection
- Perspective correction for consistent top-down view
- Grid system implementation (14x14 board)
- Automatic corner detection and alignment

### Image Processing Pipeline
1. Color space transformation (BGR to HSV)
2. Color thresholding for board isolation
3. Gaussian blur for noise reduction (15x15 kernel)
4. Binary thresholding (threshold: 130)
5. Edge detection using Canny algorithm (70, 170)
6. Perspective transform to 1260x1260 pixels

### Grid Analysis
- 90-pixel spacing for accurate tile detection
- Horizontal and vertical line detection
- Board state analysis capabilities


## How It Works
1. Takes an input image of the Mathable game board
2. Detects and isolates the board using color segmentation
3. Corrects perspective to get a perfect top-down view
4. Processes the image for clear tile detection
5. Analyzes the board state for score calculation


