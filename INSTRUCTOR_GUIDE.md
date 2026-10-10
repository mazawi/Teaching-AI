# Instructor guide — Lecture 04 practicals

## Pedagogical sequence
1. Introduce the problem and have students identify features and output type.
2. Examine the simulated dataset and graph before running a model.
3. Explain why the algorithm is suitable; challenge students to propose alternatives.
4. Execute the training or optimisation procedure one cell at a time.
5. Interpret the task-appropriate evaluation and scrutinise its limitations.
6. Modify the new-observation cell and predict what will change before rerunning.

## Suggested lesson structure
- 10 minutes: problem and data inspection.
- 15 minutes: algorithm and training.
- 15 minutes: drawing/interpreting results.
- 10 minutes: testing new inputs.
- 10 minutes: discussion and reflections.

## Assessment alignment
- **MLO1:** explanation of machine-learning approaches and real applications.
- **MLO3:** apply ML techniques to relevant data and Python software.
- **MLO4 preparation:** justify selection of algorithms according to problem and available labels.

## Notes on the labels and metrics
- Classification includes held-out accuracy, precision, recall, F1 and a confusion matrix.
- Continuous regression is evaluated with MAE, RMSE and R²; classification metrics have no defined meaning here.
- K-means uses silhouette; optional ARI compares the model with **hidden** simulated groupings, never train K-means on `synthetic_group`.
- Isolation Forest is unsupervised; artificial `is_anomaly` labels are used only after training to demonstrate precision/recall/confusion matrix.
- Association rules use support, confidence and lift rather than an inappropriate supervised confusion matrix.
- Q-learning uses rewards, learned policies and goal achievement rather than classification metrics.

All examples are synthetic, for educational purposes only. Particularly avoid interpreting GPA/salary/risk predictions as facts about real people.
