Reactive Path Planning for Low-Speed UAVs and Mobile Robots in Static Environments Using Adaptive Block Coordinate Descent Logistic Regression (ABCD-LoR)

This repository implements a reactive obstacle-avoidance method that frames static-environment navigation as a three-class classification problem (no turn / left turn / right turn). The classifier is a multinomial logistic regression model trained with an adaptive block-coordinate gradient descent optimizer (ABCD-LoR).

Key features:
- Decisions made sequentially from current infrared and ultrasonic readings (no global map required at runtime)
- Adaptive block-coordinate updates that select the parameter block with the largest estimated decrease in negative log-likelihood
- Evaluation with pseudo-R², AIC/BIC, likelihood-ratio tests, classification metrics and ROC analysis
- Simulation results on two dense static layouts at three low speeds (2.77, 13.8, 19.4 cm/s)
- Comparison against A*, VFH, Fuzzy Logic Controller, Dynamic Window Approach, Artificial Potential Fields and ASGD-trained logistic regression

Note: Results are based on a small simulated dataset (292 samples), rule-generated labels and noise-free sensors. Further real-world validation is required before deployment on actual UAVs or robots.
