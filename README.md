# 🌌 Starry Night Cellular Automaton

*A Starry Night Cellular Automaton* is inspired by the swirling skies of Van Gogh’s **The Starry Night**. The screen is filled with tiny “cells,” each functioning like a pixel in a living painting. At any moment, a cell can come alive as a glowing swirl of light that drifts and fades, creating a constantly evolving star field.

Each cell behaves like a small pseudo–finite state machine with four main states: **inactive**, **birth of the star**, **star swirl**, and **fading**. It’s called a pseudo FSM because the first state transition—from inactive to birth—is driven by randomness rather than fixed rules. This randomness gives the simulation a natural, spontaneous feel, like stars blinking into existence.

The real cellular automaton behavior begins once a cell enters the **star swirl** state. Unlike traditional automata, which apply fixed rules across a uniform neighborhood, this system uses a more flexible, local approach. If a cell is surrounded by roughly three active swirling neighbors, it will likely begin to swirl as well. This interaction isn’t global but rather specific to each cell and its immediate conditions, giving the swirls an organic, self-propagating quality.

Once swirling, a cell chooses a direction and a color, influenced by **Van Gogh’s palette**, and pushes its energy outward. It gradually loses intensity over time, guided by a global fade rate. As it fades, the cell enters the **fading** state, and eventually returns to being **inactive**, completing its life cycle.

