# Predicting MIDI drum performance style and drummer

This is a project of music analytics course (LTAT.02.015) in University of Tartu.

Data is from here: https://magenta.tensorflow.org/datasets/groove

We try to predict style and drummer of MIDI drum performances in the following way:

1. Find maximum and minimum values of all note velocities in the training dataset.
2. Divide the range between min and max value into N bins.
3. For each MIDI file, count how many note velocities fall into each bin and normalize.
4. Use normalized bin values as features for classification.
