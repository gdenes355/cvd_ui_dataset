# Investigating Color-Blind User-Interface Accessibility via Simulated Interfaces

## abstract
Over 300 million people who live with color vision deficiency (CVD) have a decreased ability to distinguish between colors, limiting their ability to interact with websites and software packages. User interface designers have taken various approaches to tackle the issue with most offering a high contrast mode. The Web Content Accessibility Guidelines (WCAG) outline some best practices for maintaining accessibility that have been adopted and recommended by several governments; however, it is currently uncertain how this impacts perceived user functionality and if this could result in a reduced aesthetic look. In the absence of subjective data, we aim to investigate how a CVD observer might rate the functionality and aesthetics of existing UIs. However, the design of a comparative study of CVD vs. non-CVD populations is inherently hard, therefore we build on the successful field of physiologically-based CVD models, and propose a novel simulation-based experimental protocol, where non-CVD observers rate the relative aesthetics and functionality of screenshots of 20 popular websites as seen in full color vs. with simulated CVD. Our results show that relative aesthetics and functionality correlate positively and that an operating-system-wide high contrast mode can reduce both aesthetics and functionality. While our results are only valid in the context of simulated CVD screenshots, the approach has the benefit of being easily deployable, and can help to spot a number of common pitfalls in production. Finally, we propose a AAA-A classification of the interfaces we analyzed.

## repository structure
* `screenshots/*.png`: the set of screenshots used during the experiment
* `data_clean.csv`: experiments results

## experiment trials
In each trial, observers had to rate the relative functionality and aesthetics of the screenshots that were identical in terms of content, but have been distorted with color blindness (CVD) filters.

## data_clean.csv
Each row contains the following information:
* `session`: UUID of the participant
* `stimulus`: unique name of the stimulus that encodes the app name, the screenshot number and whether high-contrast mode was used. This information is also encoded in subsequent columns
* `func`: functionality score from `1` to `5`, where `5` means that CVD-simulated images seem equally usable/functional
* `aes`: aesthetics score (`0` or `1`), where `1` means that CVD-simulated images seem equally aesthetic (orderly, clean, beautiful)
* `app`: name of the application
* `hc`: was the Windows high-contrast theme enabled? This only affects the CVD-simulated images
* `ref`: path to the reference image that was shown in the trial
* `deut`: path to the CVD-simulated image that mimics what a color blind user with deuteranopia would see.
* `prot`: path to the CVD-simulated image that mimics what a color blind user with protanopia would see.
* `trit`: path to the CVD-simulated image that mimics what a color blind user with tritanopia  would see.

## Data collection methodology
For a complete description of the data collection, please see our paper at [MDPI Computers](https://doi.org/10.3390/computers13020053)

## References, license
We welcome the use of our dataset and results in any subsequent study. Please remember to cite our article as follows:
```
Jamil, A.; Denes, G. Investigating Color-Blind User-Interface Accessibility via Simulated Interfaces. Computers 2024, 13, 53. https://doi.org/10.3390/computers13020053
```

