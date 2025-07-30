# 🧪 Process Optimization in Color-Sensitive Manufacturing

This repository documents a project focused on validating regression models for process optimization in the manufacturing of color-sensitive polycarbonate compounds. The work is based on the methods presented in the academic paper, *"Designing Experiments: 3 Level Full Factorial Design and Variation of Processing Parameters Methods for Polymer Colors."*

The primary goal was to apply the regression models from the study to a self-designed experimental setup, calculate the predicted colorimetric deviations (dL\*, da\*, db\*), and compare the findings to validate the models' accuracy and robustness[cite: 17, 18].

## 📊 Methodology

### Design of Experiments (DOE)

A **three-level full factorial design** was used to investigate the impact of three critical processing parameters on the final product color[cite: 7, 21]. This approach allows for a systematic analysis of both the individual and interactive effects of the variables[cite: 23, 28].

The three process parameters and their experimental levels were:
* **Temperature**: 230°C (-1), 255°C (0), 280°C (+1) [cite: 38]
* **Speed**: 700 rpm (-1), 750 rpm (0), 800 rpm (+1) [cite: 38]
* **Feed Rate**: 20 kg/h (-1), 25 kg/h (0), 30 kg/h (+1) [cite: 38]

### Regression Modeling

The predictive regression equations from the source article were used to calculate the colorimetric properties (dL\*, da\*, db\*) for each of the 27 unique experimental conditions[cite: 26, 29, 46].

The uncoded regression equations used are as follows:

* **dL\***:
    dL* = 63.86 - 0.1965*Temp - 0.06509*Speed - 0.9948*Feed Rate + 0.000184*Temp*Speed + 0.001966*Temp*Feed Rate + 0.000640*Speed*Feed Rate` [cite: 54]

* **da\***:
    da* = 14.60 - 0.01850*Speed - 0.4730*Feed Rate + 0.000598*Speed*Feed Rate` [cite: 59]

* **db\***:
    db* = 4.087 - 0.004789*Speed - 0.02975*Feed Rate` [cite: 64]

## 📈 Results and Discussion

The predicted values for dL\*, da\*, and db\* calculated using the regression models generally aligned with the trends reported in the source article, confirming the models' validity and robustness[cite: 73, 79].

Minor discrepancies between the calculated results and the article's findings were observed[cite: 74]. These are likely attributable to several factors:
* **Dataset Variations**: The initial dataset contained redundancies from repeated experimental runs, which were cleaned to ensure data integrity[cite: 33, 87].
* **Numerical Precision**: The regression coefficients in the original paper may have been rounded, leading to small differences in predicted outcomes[cite: 89].
* **Measurement Errors**: Potential variability in original colorimetric measurements could introduce slight errors[cite: 90].

## 🏭 Conclusion and Future Directions

This experiment successfully validated the use of chemometric modeling as a powerful tool for process optimization, demonstrating that product quality can be reliably predicted without extensive physical testing[cite: 92, 93]. 
This is especially valuable in industries like plastics and coatings where color consistency is critical[cite: 94].

### Future Work
To build upon this study, future efforts could include:
* **Additional Factors**: Incorporating more variables like material composition or environmental conditions to enhance the model's predictive power[cite: 97].
* **Machine Learning**: Applying advanced models like artificial neural networks (ANNs) to capture more complex, non-linear relationships[cite: 98].
* **Expanded Properties**: Extending the analysis to other key product properties such as texture, gloss, or mechanical strength for a more holistic optimization model[cite: 99].
