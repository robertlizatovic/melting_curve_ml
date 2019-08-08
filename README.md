# Machine learning of protein thermal stability
This project aims to develop algorithms that can infer protein stabilities (i.e. melting points - **Tm**) from their thermal unfolding curves as well as distinguish good curves from noisy ones (low signal-to-noise ratio)

## Tm determination using DSF (differential scanning fluorimetry)
Protein thermal stabilities (**Tms**) are defined as the temperatures at the inflection points (maximum value of the derrivative) of DSF curves. In some cases, due to the presence of contaminants and low signal-to-noise ratios, the inference of **Tms** from these curves can be difficult. In this repo I investigate the use of various machine learning and particularily deep learning techniques to automatically infer protein stabilities from the DSF curves (1D signals)

## The benchmark set
To obtain the training data for supervised learning, I simulate various real-world scenarios (low signal, presence of contaminants, multiple transition points etc.) to generate a large dataset of curves for benchmarking the algorithms.

## ML approaches
Here I investigate the performance of various classic ML techniques like random forests for classifying the DSF curves and computing the predicted stabilities from them.

## Deep learning approaches
Here I use neural nets (particularily CNNs due to the locality of the DSF signal) to develop an algorithm that can both classify the DSF curves and determine the stabilities from the ones that pass the quality check.
