# Freeway Movement Model

This repository contains a MATLAB-based simulator to mimic mobility using the Freeway Movement model. In this model, movement mainly follows a straight path, resembling the movement on freeways or highways. The direction, once established, remains consistent, emphasizing straight-line movement.

## Description

The function `freewayMovement` simulates the movement of a node (e.g., a vehicle) on a freeway. A unique feature of freeway movement is that once a direction is chosen, it remains fixed, simulating the uninterrupted straight paths of freeways.

- The speed of the node is randomized between typical freeway speeds.
- Direction is determined once and remains unchanged throughout the simulation.
- The model can be used to study communication scenarios on highways, where there's minimal deviation from a straight path.

## Prerequisites

Make sure you have MATLAB installed on your computer. Additionally, ensure any required packages or dependencies (like `myPackageConstant`) are in the MATLAB path or the current directory.

## Usage

1. Clone this repository.
2. Navigate to the directory containing `freewayMovement.m`.
3. In MATLAB, you can use the function as:

```matlab
initialPosition = struct('x', 0, 'y', 0, 'd1', 0);
rxHeight = 2;  % For example
newPosition = freewayMovement(initialPosition, rxHeight);
