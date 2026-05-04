# CPU & GPU Thermal Performance Analysis Under Real-World Workloads

## Overview
This project analyzes CPU and GPU performance under different workloads (idle, gaming, and stress) using real hardware telemetry data. The goal is to understand how system components respond thermally and behaviorally under increasing load conditions.

Data was collected using system monitoring tools and processed using Python for cleaning, transformation, and visualization.

## Tools & Technologies
- Python
- Pandas
- Matplotlib
- Intel Extreme Tuning Utility (CPU data)
- GPU monitoring tools (MSI Afterburner / FurMark-style logs)

## Workflow
1. Collected CPU and GPU telemetry under:
  - Idle
  - Gaming
  - Stress conditions
2. Cleaned and standardized raw hardware logs
3. Handled non-standard GPU log formats (.hml)
4. Processed datasets using Pandas
5. Visualized thermal and performance behavior using Matplotlib

## Key Insights
- CPU temperature increased significantly under stress workloads compared to idle and gaming conditions
- GPU exhibited stronger thermal spikes under sustained stress testing
- Power consumption strongly correlated with temperature increases in both CPU and GPU
- System cooling showed stable but delayed response under full load conditions

## Skills Demonstrated
- Data cleaning from raw hardware logs
- Handling non-standard file formats
- Time-series performance analysis
- Data visualization
- System performance interpretation

## Purpose
This project demonstrates real-world hardware performance analysis using Python, simulating the type of workload analysis used in systems engineering and performance optimization roles.
