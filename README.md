# KaxxParticles

KaxxParticles is a Java project that allows you to create and manage particle effects in Minecraft. It provides a simple and intuitive API for creating, configuring, and displaying particle effects in the game.

## Features

- Create particle effects with various parameters such as type, location, offset, speed, count, and additional data.
- Display particles at a long distance.
- Send a packet to a player to display particles at a specific location.

## Usage

Here is a basic example of how to use KaxxParticles:

```java
// Create a new particle effect
EnumParticle particleType = EnumParticle.SMOKE_NORMAL;
Location location = new Location(world, x, y, z);
KaxxParticles particles = new KaxxParticles(particleType, location);

// Send the particle effect to a player
Player player = Bukkit.getPlayer("playerName");
particles.send(player);
```

## Pros and Cons

### Pros

- Easy to use: KaxxParticles provides a simple and intuitive API for creating and displaying particle effects.
- Customizable: You can configure various parameters of the particle effects such as type, location, offset, speed, count, and additional data.
- Lightweight: KaxxParticles is a lightweight library that does not require any external dependencies.
- Fast: KaxxParticles is optimized for performance and can display particles at a long distance.
- Versatile: KaxxParticles supports a wide range of particle types and can be used in various scenarios.

### Cons

- Limited features: KaxxParticles is a basic library that provides only the essential functionality for creating and displaying particle effects.
- No built-in support for custom particles: KaxxParticles does not support custom particle effects out of the box, but you can create custom particles by extending the existing classes.
- No support for particle trails: KaxxParticles does not provide built-in support for creating particle trails, but you can achieve this by sending multiple particle packets in sequence.
- No support for particle animations: KaxxParticles does not provide built-in support for creating animated particle effects, but you can achieve this by sending multiple particle packets with different parameters.

## Requirements

- Java
- Kotlin
- Gradle

## Building

This project uses Gradle for building and managing dependencies. To build the project, navigate to the project directory and run the following command:

```bash
./gradlew build
```

## Contributing

Contributions are welcome! Please read the contributing guidelines before getting started.