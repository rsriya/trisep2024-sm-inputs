# Inputs for the TRISEP 2024 Standard Model Lectures

## Muon decay data

This is contained in the file ```muon_data_cleaned.dat```. This data file contains two columns. The first is the time in nanoseconds between the pulses of light in an experiment, the first pulse "triggering" the experiment to record data and the second pulse indicating the experiment should stop counting and reset. The pulses are expected to be generated when a muon with <160 MeV of energy slows and stops in the experiment. Stopping releases energy as the muon ionizes the medium, and this generates the first pulse. The muon will then decay at rest in an average time of about 2 microseconds (2000 nanoseconds). The second pulse results from the decay process. The time between pulses is the observed "lifetime" of the muon.

You can use this data and a model and attempt to fit for the lifetime of the muon. A good baseline model for the decay process is

$$ P(t) = A e^{-\lambda t} + B $$

The model has three free parameters whose values need to be determined from the data: the multiplicative constant of the exponential decay function (A), the decay parameter ($\lambda$) related to the lifetime $\tau=1/\lambda$), and the background constant (B). Random pulses of light will occur in the experiment, and these should happen with uniform randomness with equally distributed times between random pulses. 
