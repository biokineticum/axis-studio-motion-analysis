# Demo Data Setup for GitHub Repository

## 📁 Directory Structure to Create

Add this folder structure to your GitHub repository:

```
axis-studio-motion-analysis/
├── index.html (your main app)
├── README.md
└── demo-data/
    ├── README.md
    ├── jump-analysis/
    │   ├── jump_analysis_sample.xlsx
    │   ├── athlete_jump_session.xlsx
    │   └── README.md
    ├── gait-analysis/
    │   ├── walking_analysis_sample.xlsx
    │   ├── running_gait_sample.xlsx
    │   ├── clinical_gait_sample.xlsx
    │   └── README.md
    └── sample-outputs/
        ├── jump_analysis_example.png
        ├── gait_analysis_example.png
        └── README.md
```

## 📝 Demo Data README.md

Create `demo-data/README.md`:

```markdown
# Demo Data for Axis Studio Motion Analysis

This folder contains sample datasets to test the motion analysis tool immediately.

## 🏃‍♂️ Jump Analysis Samples

### jump_analysis_sample.xlsx
- **Description**: Basic vertical jump performance data
- **Duration**: ~10 seconds with 3-4 jumps
- **Columns**: Frame, Hips-Joint-Posi-y (plus other standard Axis Studio columns)
- **Use Case**: Test basic jump detection and height calculation

### athlete_jump_session.xlsx  
- **Description**: Extended training session with multiple jumps
- **Duration**: ~30 seconds with 8-10 jumps
- **Columns**: Frame, Hips-Joint-Posi-y (plus other standard Axis Studio columns)  
- **Use Case**: Analyze jump consistency and fatigue patterns

## 🚶‍♂️ Gait Analysis Samples

### walking_analysis_sample.xlsx
- **Description**: Normal walking gait data
- **Duration**: ~15 seconds of steady walking
- **Columns**: Frame, Hips-Sensor-Acce-x/y/z, RightFoot-Sensor-Acce-x/y/z, LeftFoot-Sensor-Acce-x/y/z
- **Use Case**: Basic gait parameter calculation and symmetry analysis

### running_gait_sample.xlsx
- **Description**: Running stride analysis
- **Duration**: ~12 seconds of steady running
- **Columns**: Frame, Hips-Sensor-Acce-x/y/z, RightFoot-Sensor-Acce-x/y/z, LeftFoot-Sensor-Acce-x/y/z
- **Use Case**: Higher cadence gait analysis with increased acceleration values

### clinical_gait_sample.xlsx
- **Description**: Clinical assessment walking data with subtle asymmetries
- **Duration**: ~20 seconds of controlled walking
- **Columns**: Frame, Hips-Sensor-Acce-x/y/z, RightFoot-Sensor-Acce-x/y/z, LeftFoot-Sensor-Acce-x/y/z
- **Use Case**: Demonstrate symmetry analysis and clinical applications

## 🎯 How to Use Demo Data

1. **Download** any sample file from this directory
2. **Go to** [https://biokineticum.github.io/axis-studio-motion-analysis](https://biokineticum.github.io/axis-studio-motion-analysis)
3. **Upload** the sample file (no preparation needed - already formatted)
4. **Select** the appropriate analysis type (Jump or Gait)
5. **Click** "Run Analysis" to see results immediately!

## 📊 Expected Results

### Jump Analysis Output:
- Professional trajectory plots with detected jump peaks
- Summary statistics (total jumps, max height, average height, std deviation)
- Detailed table with timing and height data for each jump

### Gait Analysis Output:
- Multi-panel visualization (acceleration, step detection, foot sensor comparison)
- Gait metrics (cadence, step time statistics, RMS acceleration)
- Symmetry indices when foot sensor data is available

## 🔬 Data Format Notes

All demo files are:
- ✅ **Pre-processed** - First metadata row already removed
- ✅ **Excel format** - Ready for immediate upload
- ✅ **Standard columns** - Following Axis Studio naming conventions
- ✅ **Clean data** - No missing values or outliers
- ✅ **Realistic values** - Represent actual human movement patterns

## 📈 Sample Output Images

Check the `sample-outputs/` folder for example screenshots showing what your analysis results should look like.

---

**Start analyzing motion data in under 30 seconds with these samples!** 🚀
```

## 📊 Sample Data Creation Guide

### For Jump Analysis Demo Files:

Create Excel files with these columns:

* **Frame**: Sequential numbers (0, 1, 2, 3...)

* **Hips-Joint-Posi-y**: Vertical position data with clear jump patterns

  * Baseline around 1.0-1.2m
  * Jump peaks reaching 1.3-1.6m
  * Realistic jump durations (\~0.5-1.0 seconds)
  * Multiple jumps with varying heights

### For Gait Analysis Demo Files:

Create Excel files with these columns:

* **Frame**: Sequential numbers

* **Hips-Sensor-Acce-x/y/z**: Hip acceleration data

  * Realistic gait acceleration patterns
  * Periodic step signatures
  * Values typically 0.5-2.0g range

* **RightFoot-Sensor-Acce-x/y/z**: Right foot acceleration

* **LeftFoot-Sensor-Acce-x/y/z**: Left foot acceleration

  * Clear push-off peaks
  * Slight asymmetries for clinical sample

## 🎯 Action Items:

1. **Create demo-data folder** in your GitHub repository
2. **Generate sample Excel files** using realistic biomechanical data
3. **Add README files** with descriptions for each dataset
4. **Take screenshots** of analysis results for the sample-outputs folder
5. **Update main README** with links to demo data
6. **Post on social media** using the promotional content above

## 📄 License Information

**Important**: This tool is licensed for **non-commercial use only**.

### ✅ Permitted Uses:

* **Academic research** and publications
* **Educational purposes** in universities and schools
* **Personal learning** and skill development
* **Clinical research** (non-profit)
* **Student projects** and thesis work

### ❌ Not Permitted:

* **Commercial analysis services**
* **Selling analysis reports** to clients
* **Integration into paid software**
* **Business/consulting use** for profit

### 💡 Commercial Licensing:

For commercial use, please contact: \[<your-email@domain.com>]

This setup will make your tool immediately accessible to researchers and provide a professional demonstration of its capabilities! 🚀
