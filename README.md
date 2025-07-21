Axis Studio Motion Analysis Tool

A comprehensive web-based application for analyzing motion capture data exported from Axis Studio. Performs professional-grade biomechanical analysis with real-time visualization and detailed reporting.

🚀 Live Demo

Try the tool here!

📋 Features

🏃‍♂️ Jump Height Analysis

Automatic jump detection from hip position data using state-based algorithms
Professional trajectory plots with baseline thresholds and peak markers
Comprehensive statistics: total jumps, max/average heights, standard deviation
Detailed jump data table with precise timing and height measurements
Savitzky-Golay filtering for data smoothing
🚶‍♂️ Gait Analysis
Step detection from hip and foot sensor acceleration data
Multiple visualization plots: raw acceleration, step detection, foot sensor comparison
Comprehensive gait metrics: cadence, step time statistics, RMS acceleration
Symmetry analysis comparing left vs right foot sensors
Butterworth high-pass filtering to remove gravity component

🔧 Quick Start Guide

Step 1: Prepare Your Data
Export from Axis Studio: Export your motion capture data as CSV format
Open in Excel: Load the CSV file in Microsoft Excel
Remove metadata: Delete the first row (contains metadata, not data)
Save as Excel: Save the file as Excel (.xlsx) format
Upload: Use the prepared Excel file in the web application
Step 2: Run Analysis
Upload File: Select your prepared Excel file
Choose Analysis Type:
Jump Height Analysis - for vertical jump performance
Gait Analysis - for walking/running patterns
Run Analysis: Click the blue "Run Analysis" button

View Results: Comprehensive analysis with professional graphs appears instantly

📊 Understanding Your Results
Jump Analysis Output
Summary Statistics: Total jumps, maximum height, average height, standard deviation
Trajectory Plot: Hip position over time with detected jump peaks marked
Detailed Table: Individual jump data with start/peak/end times and heights
Professional Visualization: Matplotlib-style plots with baselines and peak markers
Gait Analysis Output
Gait Metrics: Steps detected, cadence (steps/min), step timing statistics
Acceleration Plots: Raw hip acceleration and filtered step detection
Foot Sensor Analysis: RMS acceleration and peak push-off forces (when available)
Symmetry Analysis: Left/right balance assessment with percentage indices
Multi-panel Visualization: 3-panel layout showing different analysis aspects

📁 Required Data Columns

For Jump Analysis:
Frame Column: Any column containing "frame" in the name
Hip Position: Hips-Joint-Posi-y (vertical hip position)
For Gait Analysis:
Hip Acceleration:
Hips-Sensor-Acce-x
Hips-Sensor-Acce-y
Hips-Sensor-Acce-z

Foot Sensors (optional, for enhanced analysis):
RightFoot-Sensor-Acce-x/y/z
LeftFoot-Sensor-Acce-x/y/z
⚙️ Analysis Settings

Jump Analysis Parameters

JUMP_SETTINGS = {
    FS: 60,                    // Sampling frequency (Hz)
    BASELINE_FRAMES: 60,       // Frames for baseline calculation  
    MIN_RISE_CM: 5,           // Minimum rise threshold (cm)
    BACK_TO_BASELINE_CM: 2    // Landing detection threshold (cm)
}


Gait Analysis Parameters

GAIT_SETTINGS = {
    FS: 60.0,                 // Sampling frequency (Hz)
    HIGH_PASS_CUTOFF: 0.5,    // High-pass filter cutoff (Hz)
    MIN_STEP_INTERVAL: 0.5    // Minimum time between steps (s)
}


🛠️ Technical Implementation

Analysis Algorithms
Jump Detection: State-based algorithm with configurable thresholds
Data Smoothing: Savitzky-Golay filter (polynomial order 3)
Peak Detection: Custom algorithm for jump apex identification
Step Detection: Butterworth high-pass filtering + peak detection
Symmetry Calculation: RMS and peak comparison between sensors
Visualization
Canvas-based Rendering: HTML5 Canvas with matplotlib-style plotting
Professional Graphs: Axes, labels, legends, and grid formatting
Real-time Display: Immediate results without server processing
Responsive Design: Works on desktop, tablet, and mobile devices
🌐 Browser Compatibility
✅ Chrome 80+
✅ Firefox 75+
✅ Safari 13+
✅ Edge 80+


📄 License

MIT License - Free for research, commercial, and educational use.
🏷️ Citation
If you use this tool in your research, please cite:

Axis Studio Motion Analysis Tool
https://github.com/yourusername/axis-studio-motion-analysis


Built for researchers, clinicians, and movement scientists working with Axis Studio motion capture data.

🎯 Perfect for:
Sports performance analysis
Research data processing
Student projects and education
Quick motion analysis needs

Start analyzing your motion data in under 2 minutes! 🚀


