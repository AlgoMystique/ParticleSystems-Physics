# Particle Systems with Acceleration and Friction.

This repository demonstrates how to create a particle system using HTML5 canvas and vanilla JavaScript, incorporating acceleration and friction based on real-world physics. The particles react to mouse movement and other interactions, simulating natural behavior using fundamental physics principles.

## ## Live Demo

Check out the live demo [here](https://algomystique.github.io/ParticleSystems-Physics)

## Features-

- **Fully Responsive Canvas**: Ensures the canvas adjusts dynamically to different screen sizes while maintaining functionality.
- **Particle Interaction**: Particles respond to mouse events, such as clicking, with realistic movement and collisions.
- **Physics-Based Movement**: Acceleration and friction are applied to particles for smooth, realistic motion.

## How Physics is Applied-

- ### Acceleration:

Each particle's velocity increases over time due to acceleration. This simulates the effect of an external force (like gravity or user interaction). The velocity is updated every frame based on acceleration values.

**Formula:**
[ {velocity} += {acceleration} ]

- ### Friction:
To simulate natural resistance (such as air drag), friction is applied, slowing down the particles over time. This gives a more realistic motion, preventing particles from moving indefinitely or too fast.

**Formula:*
[ {velocity} *= {friction_coefficient} ]

A friction coefficient slightly less than 1 (e.g., 0.98) is used to gradually reduce the particle's speed.

## Key Concepts-

- **Distance Calculation**: Determines the distance between two points on the canvas to trigger proximity-based behaviors (e.g., attraction, repulsion).
  
  **Formula:Pythagorean theorem**
  
  [{distance} = sqrt{(x_2 - x_1)^2 + (y_2 - y_1)^2} ]
  
- **Direction of Push**: Used for interactive effects where the particles react to user input by "pushing" particles away or attracting them.
  
  **Formula:**
  [ {angle} = {Math.atan2}(dy, dx)]

## How It Works-

**Canvas Setup:** A responsive HTML5 canvas is initialized, and particles are randomly generated with positions, velocities, and accelerations.

**Particle Motion:** Each particle’s velocity is updated according to its acceleration, and friction is applied to simulate resistance. The direction of movement is calculated based on user interaction or random initial values.

**Rendering:** Every frame, particles are drawn on the canvas, and their positions are updated according to the laws of motion.

**Mouse Interaction:** When the user moves the mouse or clicks on the canvas, the particles react by accelerating away or towards the pointer.

## Technologies Used-

- HTML5 Canvas

- CSS3

- Vanilla JavaScript

## License

This project is licensed under the MIT License. See the LICENSE file for more information.
