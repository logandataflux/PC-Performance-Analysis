# **CPU & GPU Thermal Performance Analysis Under Real-World Workloads**

## **Overview**
This project analyzes CPU and GPU performance under different workloads (idle, gaming, and stress) using real hardware telemetry data. The goal is to understand how system components respond thermally and behaviorally under increasing load conditions.

Data was collected using system monitoring tools and processed using Python for cleaning, transformation, and visualization.

## **Data Collection Methodology**
### **CPU Data Collection:**

CPU performance data was collected using Intel Extreme Tuning Utility (XTU) under three controlled workload conditions: 

- Idle Test: System left idle with background processes minimized to measure baseline thermal and power behavior. 
- Gaming Simulation: System was monitored while running a GPU-intensive game scenario to simulate typical real-world gaming load on the CPU. 
- Stress Test: CPU stress testing was performed using Intel XTU built-in stress tools to simulate sustained maximum workload across all cores.

All CPU metrics (temperature, usage, power draw, frequency) were logged in real time.

### **GPU Data Collection:**

GPU performance data was collected using real-time hardware monitoring tools during controlled workload scenarios: 

- Idle Test: GPU remained at desktop with minimal background activity to capture baseline power and thermal state. 
- Gaming Test: A 3D rendering workload was executed at 1920×1080 resolution, 144Hz refresh rate, with DLSS disabled, to simulate a consistent high-performance gaming scenario. 
- Stress Test: A GPU stress benchmark (FurMark-style workload) was used to generate sustained maximum load and thermal output.

GPU metrics collected included temperature, usage, clock speeds, memory usage, power draw, and fan response.

### **Environment Conditions:**
Resolution: 1920×1080 (Gaming test)
Refresh Rate: 144Hz
DLSS: Disabled
Power plan: High performance
Background applications minimized
Consistent ambient room conditions (non-controlled but stable environment)

## **Tools & Technologies**
- Python
- Pandas
- Matplotlib
- Intel Extreme Tuning Utility (CPU data)
- GPU monitoring tools (MSI Afterburner)

## **Workflow**
1. Collected CPU and GPU telemetry under:
  - Idle
  - Gaming
  - Stress conditions
2. Cleaned and standardized raw hardware logs
3. Handled non-standard GPU log formats (.hml)
4. Processed datasets using Pandas
5. Visualized thermal and performance behavior using Matplotlib

## **Key Insights**
- CPU temperature increased significantly under stress workloads compared to idle and gaming conditions
- GPU exhibited stronger thermal spikes under sustained stress testing
- Power consumption strongly correlated with temperature increases in both CPU and GPU
- System cooling showed stable but delayed response under full load conditions

## **Skills Demonstrated**
- Data cleaning from raw hardware logs
- Handling non-standard file formats
- Time-series performance analysis
- Data visualization
- System performance interpretation

## **Purpose**
This project demonstrates real-world hardware performance analysis using Python, simulating the type of workload analysis used in systems engineering and performance optimization roles.
