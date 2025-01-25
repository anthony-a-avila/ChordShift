# ChordShift

## Overview
ChordShift is a Python-based tool designed to help musicians and composers explore unique harmonic combinations using algorithmic generation. By leveraging pitch-class sets within the 12-tone equal temperament system, ChordShift enables users to discover novel harmonic ideas and expand their musical vocabulary.

This project compares two search algorithms, A* and Simulated Annealing, to generate intermediate chords that satisfy user-defined harmonic constraints. Users can define their preferences for consonance or dissonance, making the tool highly customizable, but also agnostic to subjective musical preferences.

---

## Features
- **Harmonic Exploration**: Focuses on unique note combinations (pitch-class sets) rather than permutations to explore a wide harmonic space.
- **User Customization**: Agnostic to specific musical styles, enabling users to define consonance or dissonance scores.
- **Algorithmic Comparison**: Implements and compares the performance of A* global search and Simulated Annealing local search for chord generation.
- **Brainstorming Aid**: Designed as a tool for musicians to "re-roll the dice" and discover inspiring chord progressions.

---

## Technical Details
### Algorithms
1. **A***: A global search algorithm that finds an optimal solution by exploring multiple paths using a heuristic evaluation function. In this case, the heuristic is calculated by finding the minimum edit distance from one pitch-class set to another.
2. **Simulated Annealing**: A local search algorithm inspired by annealing in metallurgy, capable of escaping local optima to find near-optimal solutions.

### Evaluation Function
- Uses a dissonance metric to evaluate chords and transitions, influenced by user-defined rankings of harmonic intervals.
- The program generates intermediate chords that meet the dissonance level of predefined chord progressions.

---

## Future Work
- Incorporate more complex harmonic evaluation, including chord voicings and inversions.
- Expand to probabilistic, data-driven approaches for broader cultural relevance.
- Integrate with digital audio workstations (DAWs) for real-time musical idea generation.
