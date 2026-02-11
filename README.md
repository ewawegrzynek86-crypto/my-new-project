EUNOIA – A System Supporting Cognitive Autonomy and Stress Regulation

Final project for the Building AI course

Summary

EUNOIA is a personal artificial intelligence system designed to work alongside a wearable device in order to support cognitive autonomy through the analysis of individual physiological patterns and, optionally, linguistic patterns. The system operates locally, under full user control, and reports only correlations and trends—never causes, diagnoses, or judgments.

Background

Contemporary digital and professional environments are characterized by constant stimulation, rapid information exchange, and sustained cognitive pressure. Chronic stress and gradual overload are among the most common factors negatively affecting psychological well-being in industrialized societies.

Many individuals:

fail to recognize early signs of overload,

experience manipulative communication patterns (such as subtle invalidation of perception),

operate under gradually increasing chronic tension,

struggle with emotional regulation, particularly in the case of neurodivergent individuals.

Existing technological solutions primarily focus on generalized relaxation exercises or static self-help programs. There is a lack of systems capable of learning the unique regulatory patterns of a specific individual rather than comparing them to population-level averages.

The idea was motivated by the observation that many individuals lack tools supporting reflective awareness without imposing interpretation or external judgment. EUNOIA aims to support autonomy rather than replace it.

How is it used?

EUNOIA operates on two functional layers:

1. Continuous Physiological Calibration (Local)

The system analyzes:

heart rate (HR),

heart rate variability (HRV),

breathing rhythm (if available),

activity levels,

recovery time to baseline.

Based on these signals, EUNOIA builds an individual regulatory baseline specific to the user. Physiological signals are treated strictly as measurable biological data and are not directly interpreted as emotional states.

2. On-Demand Linguistic Analysis

The user may voluntarily submit a short text or fragment of a conversation. The system:

generates a semantic vector representation of the text,

compares linguistic patterns with locally stored representations (if enabled),

correlates linguistic patterns with physiological data from the same time frame,

returns a neutral correlation-based report.

EUNOIA does not determine causes, evaluate individuals, or assess relationships.

A soft alert may be generated only when a stable and sustained deviation from the user’s baseline is detected.

Stakeholders and Context

The primary stakeholders are end-users seeking improved self-awareness in high-stress environments. Secondary stakeholders include developers, data protection auditors, and researchers evaluating ethical AI deployment. The system is designed to operate in personal daily contexts without external data access or institutional oversight.

Data Sources and AI Methods
Data Sources

Physiological data:

HR,

HRV,

breathing rhythm,

activity levels,

regulatory recovery time.

Linguistic data (on-demand only):

manually entered text,

speech converted to text.

The system’s effectiveness depends on the quality and consistency of physiological signals collected by consumer wearable devices. Variability in sensor accuracy may influence the reliability of trend detection.

AI Methods

unsupervised anomaly detection relative to an individual baseline,

short-term and long-term trend modeling,

semantic vector representations for linguistic analysis,

threshold-based activation mechanisms,

separation of global models and personal on-device models.

EUNOIA – Data Flow

Step 1: Physiological Data Collection

Wearable device →
• HR
• HRV
• activity
• (optional) breathing

Data is transferred locally to the application.

↓

Step 2: Local Calibration Module

New data is compared with the user’s personal baseline.
The system maintains a model of what is regulatory “normal” for this individual.

↓

Step 3: Deviation Detection

An anomaly detection module evaluates whether changes are:

temporary,

repetitive,

part of an emerging trend.

A deviation is marked as a trend only if it persists across at least three consecutive analytical periods.

No interpretation of causes is performed.

↓

Step 4: Optional Linguistic Module

The user voluntarily submits text.
A semantic representation is generated and analyzed in correlation with concurrent physiological signals.

↓

Step 5: Data Fusion

Biological and linguistic data are combined within a correlation framework.
EUNOIA applies a causal barrier principle: the system reports correlations only, never causal explanations.

↓

Step 6: Reporting and Confidence Level

The user receives:

gentle alerts only for stable trends,

a visual map of changes,

a confidence level (low / medium / high).

↓

Step 7: Local Storage

Data remains stored locally and encrypted using a user-controlled key.

↓

Step 8: Optional Encrypted Backup

The user may enable encrypted backup secured with a recovery phrase.

Local System Architecture

Wearable device → physiological data transfer.

Biological calibration module → construction of personal baseline.

Personal regulatory model → trained exclusively on-device.

Optional linguistic module → activated only upon request.

Fusion layer → correlation-based integration.

Reporting layer → neutral presentation without evaluative language.

Local storage + optional encrypted backup → user-controlled encryption.

If a global model is used, it remains strictly separated from personal data.

Color Design and Regulatory Interface Philosophy

The visual layer of EUNOIA functions as part of regulatory design rather than branding.

The color system is intentionally restrained:

White represents cognitive neutrality and absence of imposed interpretation.

Cobalt blue symbolizes precise and controlled system intervention.

Subtle gradients reflect regulation as a process rather than a sudden corrective action.

The interface avoids high-contrast stimulation and intrusive animation. Its purpose is perceptual stability and low sensory activation.

The visual design mirrors the ethical architecture of the system: clarity, restraint, and non-intrusiveness.

Ethical Principles

1. Causal Barrier Principle
The system reports correlations and trends only—never causes or diagnoses.

2. Full User Control
Linguistic analysis is strictly user-initiated. Backup is optional. Data can be deleted at any time.

3. No Behavioral Steering
EUNOIA does not issue commands, prescribe actions, or evaluate interpersonal dynamics.

4. Model Separation
Global models (if present) are separated from personal on-device models.

5. Privacy by Design
Physiological and linguistic representations do not leave the device without explicit consent.

6. Right to Erasure
Users may delete selected data periods or reset the entire profile.

Challenges

EUNOIA does not:

diagnose psychological conditions,

determine causes of emotional responses,

evaluate interpersonal relationships,

replace professional psychological support.

Limitations include:

potential false positives,

possible user over-interpretation,

limitations of linguistic models in handling irony and ambiguity,

risk of over-reliance on technological support,

the need to maintain high-level privacy safeguards.

The system reports correlations and trends only.

What Next?

Future development may include:

building a functional wearable prototype,

interface refinement,

pilot studies with real users,

ethical audits and data security testing,

interdisciplinary collaboration between AI engineers, physiologists, and ethics researchers,

refinement of trend analysis without reduction to simplistic numerical scoring.

Acknowledgments

This project is inspired by:

research on heart rate variability (HRV),

on-device processing architectures,

contemporary discussions on ethical AI design,

an original visual concept grounded in individual perceptual experience.
