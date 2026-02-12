# EUNOIA – A System Supporting Cognitive Autonomy and Stress Regulation

Final project for the Building AI course

## Summary

EUNOIA is a personalized AI system designed to operate alongside a wearable device to support cognitive autonomy through analysis of individual physiological patterns and—optionally—linguistic patterns.  
The system functions fully locally, under complete user control, and reports only correlations and trends — never causes, diagnoses, or behavioral judgments.

## Background

Modern environments are saturated with constant stimulation, rapid communication, and sustained cognitive pressure. Many individuals:

* fail to recognize early physiological signs of overload  
* struggle to detect manipulative communication patterns (e.g., subtle invalidation)  
* operate under gradually increasing chronic tension  
* face difficulties with emotional regulation, especially neurodivergent individuals  

Existing technological tools rely mainly on generic relaxation exercises or population-level models.  
There is a clear need for systems that adapt to the individual rather than requiring individuals to conform to generalized norms.

EUNOIA is grounded in the idea that people benefit from tools which enhance reflective awareness — without interpreting, correcting, or judging their experience.

## How is it used?

EUNOIA consists of two independent functional layers:

1. Continuous Physiological Calibration (Local)  
The system analyzes:
* heart rate (HR)  
* heart rate variability (HRV)  
* breathing rhythm (if available)  
* activity level  
* recovery time to baseline  

From these signals, it constructs a personal regulatory baseline unique to the user.  
Physiological signals are treated strictly as biological measurements — not as emotional labels.

2. On-Demand Linguistic Analysis  
The user may voluntarily submit text (typed or speech-to-text).  
EUNOIA then:
* generates a semantic vector representation (embedding)  
* compares it only to the user’s previous embeddings (if enabled)  
* correlates linguistic features with physiological data from the corresponding timeframe  
* returns a neutral, correlation-based report  

Nothing is interpreted as intent, diagnosis, personality, or interpersonal meaning.  
Alerts appear only when stable deviations from the personal baseline persist.  
Confidence levels describe signal stability — not interpretative certainty.

<img src="eunoia.jpg.png" width="500">

The visual design emphasizes regulatory stability rather than branding:
* White → perceptual neutrality  
* Cobalt blue → precise, controlled intervention  
* Soft gradients → regulation as a continuous process  

The interface avoids overstimulation and prioritizes clarity and low sensory load.

## Data sources and AI methods

### Data sources

Physiological data:
* HR / HRV  
* breathing rhythm  
* activity  
* recovery time  

Optional linguistic data:
* manually entered text  
* speech-to-text input  

Variability in wearable sensors may affect signal accuracy and trend detection reliability.

### AI methods

* unsupervised anomaly detection relative to individual baseline  
* short- and long-term trend modeling  
* semantic vector representations (embeddings)  
* threshold-based alert mechanisms  
* architectural separation of global and personal on-device models  

The system operates under a strict “correlation-only” framework (causal barrier principle).

## Challenges

EUNOIA does not:

* diagnose mental health conditions  
* infer emotional causes  
* evaluate interpersonal relationships  
* replace psychological care  

Limitations include:

* potential false positives  
* risk of overinterpretation by users  
* difficulty with irony and complex social cues  
* sensor inaccuracies  
* possible over-reliance on technological mediation  

Ethically, the main challenge is ensuring that users do not mistake correlation reports for causal explanations.

## What next?

Future development may include:

* early smartwatch prototype integration  
* interface refinement  
* pilot studies with volunteers  
* interdisciplinary collaboration (AI ethics, cognitive science, HCI)  
* calibration research in anomaly detection  
* formal ethical and security review  

Long-term, EUNOIA could contribute to research on privacy-preserving affect-aware AI systems.

## Acknowledgments

Inspired by:

* HRV research and autonomic regulation studies  
* on-device machine learning architectures  
* contemporary ethical AI frameworks  
* a synesthetic perceptual concept combining color and motion  

No licensed or proprietary code was used.  
The project is conceptual and exploratory.
