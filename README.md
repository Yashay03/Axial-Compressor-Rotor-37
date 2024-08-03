# Axial-Compressor-Rotor-37
## Introduction
This README file details the Computational Fluid Dynamics (CFD) analysis of the NASA Rotor 37 using ANSYS CFX. NASA Rotor 37 is a well-known transonic axial compressor rotor used extensively for benchmarking CFD codes. This rotor features 36 blades with a tip radius of 0.5 meters and a hub-to-tip ratio of 0.7. The design point corresponds to a relative tip Mach number of 1.38, making it a valuable case study for high-speed aerodynamic performance analysis.

## Objective
The objective of this analysis is to evaluate the aerodynamic performance of NASA Rotor 37 using ANSYS CFX and compare the numerical results with available experimental data. The focus is on validating the numerical approach and assessing the accuracy of the simulation by comparing it with the experimental results.

## Methodology
### Domain and Mesh
To optimize computational resources, we utilized a single blade fluid domain mesh, leveraging the symmetrical nature of the rotor. This approach significantly reduced the computational time and resources required for the analysis. The periodic boundary conditions were applied to account for the symmetry in the circumferential direction. The mesh was generated in ANSYS TurboGrid, ensuring high-quality elements around critical regions, such as the blade leading and trailing edges, hub, and tip. The final mesh was fine-tuned to capture the complex flow features present in transonic conditions.

The mesh consisted of structured grids with a refined boundary layer to accurately capture the flow characteristics near the blade surface. The total number of nodes and elements was carefully chosen to balance accuracy and computational efficiency.

### Simulation Setup
The following key parameters and settings were used for the simulation:

### Solver: ANSYS CFX
Turbulence Model: SST (Shear Stress Transport) model <br>
Inlet Total Pressure: 101,325 Pa (at sea level) <br>
Inlet Total Temperature: 288.15 K <br>
Rotational Speed: 17,188 RPM <br>
Outlet Static Pressure: Adjusted to achieve design point flow conditions <br>

## Post-Processing
The post-processing involved extracting performance metrics such as total pressure ratio, isentropic efficiency, and mass flow rate. Since only a single blade passage was modeled, the results were scaled to represent the full 36-blade rotor. This scaling was done by multiplying the single blade results by the number of blades.

## Results and Validation
The results obtained from the CFD simulation were compared with the available experimental data for NASA Rotor 37. The key performance parameters, such as total pressure ratio and isentropic efficiency, showed a good agreement with the experimental results, validating the numerical approach. The minor discrepancies observed were within acceptable limits, indicating that the simulation accurately captured the flow physics.

## Conclusion
The CFD analysis of NASA Rotor 37 using ANSYS CFX successfully demonstrated the capability of the numerical approach to predict the aerodynamic performance of the rotor. The results showed good agreement with the experimental data, confirming the reliability of the simulation setup. The use of a single blade fluid domain mesh, coupled with appropriate scaling, proved to be an efficient method for analyzing the entire rotor's performance while minimizing computational resources.
