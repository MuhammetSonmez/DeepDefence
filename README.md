# Deep Defence

Deep Defence is a deep learning-based security system designed to detect and prevent brute-force attacks. This system analyzes abnormal activities in network traffic to identify potential threats and take proactive measures.

## Features
- **Machine Learning-Based Detection:** Uses a GRU-based model to detect anomalies.  
- **Real-Time Monitoring:** Continuously analyzes network traffic and detects attacks instantly.  
- **Customizable Rules:** Users can customize defense strategies to target specific attack types.  

## Use Cases (Cases)

### Case 1: Real Brute Force Attack
An attacker tries 20 completely different passwords in a short period.
```
[ALERT] Brute-force attack detected! Total attempts: 10
```

### Case 2: Random Nonsense Passwords
The attacker rapidly tries completely random passwords.
```
[ALERT] Rapid brute-force attack detected! Requests are too frequent.
```

### Case 3: Mixed Brute Force Attack
The attacker tries both similar and different passwords.
```
[ALERT] Brute-force attack detected! Total attempts: 10
```

### Case 4: Forgotten Password Scenario
A legitimate user forgets their password and tries slight variations.
```
[NO ALERT]
```

## Model Performance Metrics

| Metric            | Class 0 (Nonsense) | Class 1 (Meaningful) | Overall |
|------------------|------------------|------------------|---------|
| Precision       | 0.9963           | 0.9966           | 0.9965  |
| Recall          | 0.9966           | 0.9963           | 0.9965  |
| F1-score        | 0.9965           | 0.9965           | 0.9965  |
| Support        | 286864           | 286886           | 573750  |
| Accuracy        | -                | -                | 0.9965  |
| Macro Avg       | 0.9965           | 0.9965           | 0.9965  |
| Weighted Avg    | 0.9965           | 0.9965           | 0.9965  |

- **Cohen's Kappa Score:** 0.9929

## Contribution
Those who wish to contribute to the project can provide feedback using the `issues` and `pull request` sections.

