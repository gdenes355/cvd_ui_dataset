# User interface (UI) funcitonality and aesthetics for color blind (CVD) users

## abstract
Color vision deficiency (CVD, color blindness) is the failure or decreased ability to distinguish between certain colors even under normal lighting conditions. There are over 300 million people worldwide with CVD including approx. 1 in 12 men (8\%) and 1 in 250 women (0.5\%). CVD can limit a user's ability to interact with websites and software packages that are otherwise basic commodities for the average user. User interface designers have taken various approaches to tackle the issue with some interfaces offering a high-contrast mode, and others integrating color-blind awareness into their website design process. The Web Content Accessibility Guidelines (WCAG) outline some best practices for maintaining accessibility that have been adopted and recommended by several governments; however, it is currently uncertain how this impacts perceived user functionality and if this could result in a reduced aesthetic look. In our work, we present a subjective user study to measure the loss of functionality and aesthetics as potentially seen by CVD observers for 20 popular websites and software packages.
This dataset contains the results of the experiment (data_clean.csv) alongside the stimuli images.

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
For a complete description of the data collection, our paper is currently under review at MDPI

