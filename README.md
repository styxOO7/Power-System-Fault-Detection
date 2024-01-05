# Power System Fault Detection and Classification 🚨

This project aims to build machine learning models that can predict the type of fault in a transmission line, based on the current and voltage measurements. The transmission line is the most crucial part of the power system, and detecting and classifying faults is essential for ensuring the reliability and security of the power grid. ⚡
• Developed a Machine Learning model to predict the fault type in a transmission line by utilizing phase
Current and Voltage as Inputs.
• Explored Voltage and Current waveforms under no-fault conditions and various types of faulted
conditions through a range of data visualization techniques using Matplotlib.
• Trained the model on a dataset comprising 7861 rows for both symmetrical and asymmetrical fault
detection and achieved an accuracy rate of 98%.
• Built and compared the performance of different machine learning models, including logistic regression,
decision tree, random forest, and support vector machine.

## Dataset Description 📊

The dataset contains 7861 samples of current and voltage measurements from a power system with 4 generators, each pair located at each end of the transmission line. Transformers are present in between to simulate and study the various faults at the midpoint of the transmission line. The dataset has 10 columns:

- G: Ground fault indicator (0 or 1)
- C: Fault in line C indicator (0 or 1)
- B: Fault in line B indicator (0 or 1)
- A: Fault in line A indicator (0 or 1)
- Ia: Current in line A
- Ib: Current in line B
- Ic: Current in line C
- Va: Voltage in line A (in per unit value)
- Vb: Voltage in line B (in per unit value)
- Vc: Voltage in line C (in per unit value)

## Objectives of Notebook 📝

The notebook contains the following steps:

- Dataset exploration using various types of data visualization. 📈
- Build machine learning models that can predict the fault type in transmission line. 🤖
- Evaluate and compare the performance of different models. 📊

## Libraries Used 📚

The notebook uses the following Python libraries:

- pandas
- numpy
- seaborn
- matplotlib
- sklearn

## Waveforms 📉
No load Current:
![image](https://github.com/styxOO7/Power-System-Fault-Detection/assets/85895343/c443db61-a119-4a56-9651-be151cc484a0)

No load Voltage:
![image](https://github.com/styxOO7/Power-System-Fault-Detection/assets/85895343/ec42b138-915f-4deb-83e1-354de08694b9)

In a normal (No_Fault) condition Voltage or Current graph, is symmetrical and sinusoidal in nature with current and voltage 120 degree in phase shift and maximum current is approximately +100 to -100 Amperes and voltage +0.5 pu to -0.5pu

SLG Fault Current:
![image](https://github.com/styxOO7/Power-System-Fault-Detection/assets/85895343/8a6f4321-062a-4c00-83a3-5b0e12fbdcc4)

SLG Fault Voltage:
![image](https://github.com/styxOO7/Power-System-Fault-Detection/assets/85895343/6c50ee88-336a-40a5-ab16-1c058a96a213)

At a time of Line A to ground fault the current in line A increases to 10 fold approximately 1000 Ampears form normal 100 Ampears and voltage reduced. Similarly, other faults have been studied.

## Model Comparision 🤖
![image](https://github.com/styxOO7/Power-System-Fault-Detection/assets/85895343/11492d2d-6eea-416c-87f7-4f5795374bc9)

Random Forest,Decision Tree Classifier,XGB Classifier, are giving the best Result with 100 percent accuracy and is doing a great job till now in Fault Detection, than the rest of the models because it's able to predict all the signals in most efficient manner while in other models there are cases where there is actually fault but the model is not able to identify it.Logistic Regression is giving the worst accuracy
