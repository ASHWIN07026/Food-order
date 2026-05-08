## EX.NO.1 — Recent Case Study of Ethical Initiatives in Healthcare, Autonomous Vehicles and Defense

**Date:**

**Aim:**
To write a case study on recent ethical initiatives in healthcare, autonomous vehicles and defense.

---

### 1) CASE STUDY: HEALTHCARE ROBOTS

AI and robotics are rapidly entering healthcare for diagnosis, surgery, and patient monitoring. Robots help in diagnosing patients, performing surgeries, monitoring health, and reminding patients to take medications.

**Safety:** Robots must not harm patients, especially vulnerable groups like elderly and children. Investment in clinical trials is essential before deployment.

**User Understanding:** Healthcare professionals must be digitally literate to use AI tools correctly and recognize their limitations. The 'da Vinci' surgical robot requires a trained operator.

**Data Protection:** Patient data must be protected from misuse and hackers. Clear frameworks for data usage must be established to maintain public trust.

**Legal Responsibility:** When AI causes harm, liability must be clearly established. Currently, AI is used as an aide, so experts remain the liable party.

**Bias:** ML algorithms trained on limited minority data can produce biased diagnoses. For example, skin cancer detection models had less than 5% dark skin images, risking misdiagnosis.

**Equality of Access:** Digital health tools may exclude those lacking digital literacy or financial access, reinforcing existing health inequalities.

---

### 2) CASE STUDY: AUTONOMOUS VEHICLES

Autonomous Vehicles (AVs) can sense their environment and operate with little or no human input. SAE International defines six levels of driving automation from Level 0 (no automation) to Level 5 (fully autonomous).

**Public Safety:** Many assisted driving functions lack independent safety certification. In 2018, an Uber AV killed a pedestrian in Arizona, raising serious ethical concerns about testing on public roads.

**Notable Accidents:**
- Jan 2016 — Gao Yaning died in Tesla Model S crash in China while Autopilot was believed engaged.
- May 2016 — Joshua Brown died in Tesla crash in Florida while Autopilot was active.
- March 2018 — Wei Huang killed when Tesla Model X crashed due to Autopilot navigation mistake.

**Data Privacy:** Manufacturers collect large amounts of AV data. Tesla was criticized for sharing drivers' private data with media without permission after crashes.

**Employment:** AVs threaten jobs of bus, taxi, and truck drivers. In 2016, the first commercial delivery using a self-driving truck was completed covering 120 miles with no human action.

**Legal Responsibility:** It is unclear who is responsible when an AV causes injury — the manufacturer, programmer, or driver. Responsibility sharing among engineers, drivers, and the AV system itself has been proposed.

---

### 3) CASE STUDY: WARFARE AND WEAPONISATION

AI is transforming modern warfare through satellite imagery analysis, cyber defense, and autonomous weapons.

**Lethal Autonomous Weapons (LAWS):** Russia has approved a plan for 30% of combat power to be autonomous by 2030. LAWS can independently search and engage targets, raising serious ethical concerns.

**Drone Technologies:** A high-quality drone costs only $1,000 compared to $100 million for a military aircraft. This makes large-scale autonomous attacks more accessible and dangerous.

**Mobile Robotic IEDs:** Self-driving technology could be misused to deliver explosives precisely without a human driver, making attacks more frequent and devastating.

**Ethical Concerns in Warfare:**
- Automated weapons may violate International Humanitarian Law.
- AI cannot distinguish between combatants and civilians.
- AI cannot judge whether force used is proportional.
- Delegating life or death decisions to machines violates human dignity.
- Accountability for war crimes must fall on the programmer and commanding officer.

---

**Result:**
Thus the case study on recent ethical initiatives in healthcare, autonomous vehicles and defense was completed successfully.

EX.NO.3 — Experiment the Regression Model Without Bias and With Bias
Date:

Aim:
To write a Python program to experiment the regression model without bias and with bias.

Algorithm:
Import required libraries
Generate example data
Fit regression model without bias
Fit regression model with bias
Display model parameters and output
Program:
import numpy as np
import matplotlib.pyplot as plt
from sklearn.linear_model import LinearRegression

np.random.seed(0)
X = np.random.rand(100, 1)
y = 2 + 3 * X + np.random.randn(100, 1)

# Without bias
model_no_bias = LinearRegression(fit_intercept=False)
model_no_bias.fit(X, y)

# With bias
model_with_bias = LinearRegression(fit_intercept=True)
model_with_bias.fit(X, y)

plt.figure(figsize=(12, 6))
plt.scatter(X, y, label='Data points')
plt.plot(X, model_no_bias.predict(X), color='red', label='Without bias')
plt.plot(X, model_with_bias.predict(X), color='blue', label='With bias')
plt.legend()
plt.title('Linear Regression Model with and without Bias')
plt.xlabel('X')
plt.ylabel('y')
plt.show()

print("Model parameters without bias:")
print(f"Slope: {model_no_bias.coef_[0][0]}")
print("\nModel parameters with bias:")
print(f"Intercept: {model_with_bias.intercept_[0]}")
print(f"Slope: {model_with_bias.coef_[0][0]}")

Output:
Model parameters without bias:
Slope: 6.363033406072774

Model parameters with bias:
Intercept: 2.2221510774472293
Slope: 2.9369350214020384

Result:
Thus the Python program for regression model with and without bias was executed successfully.