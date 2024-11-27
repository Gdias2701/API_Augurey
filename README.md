# Augurey API 

<p align="justify">
  
The **Augurey API** classifies the degradation stages of mechanical components based on vibration data. Its purpose is to assist in predictive maintenance, preventing catastrophic failures.
</p>

---

## Motivation
![Augurey](images/image.png)

<p align="justify">
  
The name **Augurey** refers to a bird that foretells imminent changes, much like the API alerts about the progression of mechanical component degradation. The goal is not just to predict the end of the component’s life cycle but also to prepare the maintenance team to act proactively and avoid failures in associated systems.
</p>

---

## Table of Contents  
- [Overview](#overview)  
- [How to Use](#how-to-use)  
- [Result Details](#result-details)  
- [Practical Example](#practical-example)  
- [Motivation](#motivation)  
- [References](#references)  

---

## Overview  
The API takes the following inputs:  
1. **Sampling frequency** (in Hz).  
2. **Interval between collections** (in seconds).  
3. **Collection window size** (in seconds).  
4. **CSV files containing vibration time series** (vertical and horizontal directions).  

**Output**: Classification into 4 degradation stages, with detailed analysis and degradation evolution charts.

---

## How to Use

### Step 1: Enter Collection Parameters
- Sampling frequency: Example `25600 Hz`.  
- Interval: Example `10 s`.  
- Window size: Example `0.10 s`.

### Step 2: Upload CSV Files
- Vertical file: Example `FEMTO_Test_B33V.csv`.  
- Horizontal file: Example `FEMTO_Test_B33.csv`.  
- **Maximum file size**: 200 MB.  

### Step 3: Process Data
1. Click **Submit**.  
2. The API will process the data and display the analysis results.

---

## Result Details

### Degradation Stages
- **Health + Stage 1**: Almost zero degradation, with no apparent defects.  
- **Stage 2**: Minor degradation.  
- **Stage 3**: Intermediate degradation.  
- **Stage 4**: Severe (urgent corrective action required).  

### Information Provided
1. **Time spent in each stage**:
   - Example: Stage 1 -> `21 minutes`.  
2. **Time intervals for each stage**:
   - Example: Stage 0 -> `Start: 0h, End: 3min`.  
3. **Current stage and probability**:
   - Example: Stage 3 with 90% probability.  
4. **Degradation evolution chart**.  

---

## Practical Example

### Input Configuration
- Sampling frequency: `25600 Hz`.  
- Interval: `10 s`.  
- Window size: `0.10 s`.  
- Files:
  - Vertical: `FEMTO_Test_B33V.csv`.  
  - Horizontal: `FEMTO_Test_B33.csv`.  

### Output
- **Current Stage**: 3.  
- **Probability**: 90%.  
- **Time in Stage 3**: 16 minutes.  
- **Recommended Action**: Immediate corrective maintenance.


An example of the API application is available through the link: https://www.youtube.com/watch?v=WnBlYhpmL-4

---

## References
1. Tianwen Zhu, Yongyi Ran, Xin Zhou, and Yonggang Wen, *A Survey of Predictive Maintenance: Systems, Purposes and Approaches*, arXiv preprint arXiv:1912.07383, 2024. [DOI](https://doi.org/10.48550/arXiv.1912.07383).

2. Nie, L., Zhang, L., Xu, S., et al., "Remaining useful life prediction for rolling bearings based on similarity feature fusion and convolutional neural network", *Journal of the Brazilian Society of Mechanical Sciences and Engineering*, vol. 44, pp. 328, 2022. [DOI](https://doi.org/10.1007/s40430-022-03638-0).

3. C. Scheffer and P. Girdhar, *Practical Machinery Vibration Analysis and Predictive Maintenance*. Elsevier, 2004.

4. Juodelyte, D., Cheplygina, V., Graversen, T., and Bonnet, P., "Predicting Bearings' Degradation Stages for Predictive Maintenance in the Pharmaceutical Industry", 2022. [DOI](https://doi.org/10.48550/arXiv.2203.03259).

5. Baheti, B., Huang, Q., Tian, L., Zhang, L., and Wang, K., "Fault Detection for Equipment in Distribution Grid Station House Based on Ubiquitous Internet of Things," *IEEE Xplore*, 2024. Accessed: 2024-09-24.

6. Massaro, A., Manfredonia, I., Galiano, A., Pellicani, L., & Birardi, V., "Sensing and Quality Monitoring Facilities Designed for Pasta Industry Including Traceability, Image Vision and Predictive Maintenance," *2019 II Workshop on Metrology for Industry 4.0 and IoT (MetroInd4.0&IoT)*, 2019. [DOI](https://doi.org/10.1109/metroi4.2019.8792912).

7. IEEE PHM 2012 Prognostic Challenge. Outline, Experiments, Scoring of Results, Winners, 2012. [Link](https://pt.scribd.com/document/344094074/IEEEPHM2012-Challenge-Details-Results-and-Winners).

8. Nectoux, P., Gouriveau, R., Medjaher, K., Ramasso, E., Chebel-Morello, B., Zerhouni, N., and Varnier, C., "PRONOSTIA: An Experimental Platform for Bearings Accelerated Degradation Tests," *IEEE International Conference on Prognostics and Health Management (PHM)*, pp. 1–8, 2012.

9. Iunusova, E., Gonzalez, M. K., Szipka, K., and Archenti, A., "Early fault diagnosis in rolling element bearings: Comparative analysis of a knowledge-based and a data-driven approach," *Journal of Intelligent Manufacturing*, vol. 35, pp. 2327–2347, 2024, Springer. [DOI](https://doi.org/10.1007/s10845-023-02151-y).

10. Barandas, M., Folgado, D., Fernandes, L., et al., "TSFEL: Time Series Feature Extraction Library," *SoftwareX*, vol. 11, p. 100456, 2020. [DOI](https://doi.org/10.1016/j.softx.2020.100456).

---

🍿 [Augurey inspiration (Harry Potter Wiki)](https://harrypotter.fandom.com/wiki/Augurey)

- Ready to implement and analyze with **Augurey API**! 🎉 For questions, feel free to open an *issue*. 😊

---

# Citation

If this repository helps you in any way, consider citing our paper as follows:

```bibtex
@unpublished{Gean2024Augurey_API,
  author    = {Francisco G. D. da Silva Filho and Joaquim O. F. Moura Filho and Vandilberto P. Pinto and Márcio A. B. Amora},
  title     = {Remote Monitoring of Bearing Degradation with Computational Intelligence: IoT-Integrated API for Predictive Analysis and Maintenance.},
  note      = {In preparation},
  year      = {2024},
  organization = {Federal University of Ceará},
}

