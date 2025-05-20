### Basic Lighting Types

<details>
  <summary><b>Q: What are the 5 main types of lights available in Unreal Engine 5?</b></summary>
  A: Point Light, Spotlight, Rectangle Area Light, Directional Light, and Skylight
</details>

<details>
  <summary><b>Q: What is a Point Light and how does it work?</b></summary>
  A: A Point Light emanates from a single point outward in all directions. It's the simplest type of light where light spreads uniformly from a central point.
</details>

<details>
  <summary><b>Q: How does a Spotlight differ from a Point Light?</b></summary>
  A: A Spotlight has directionality and emanates from a point, similar to real-world halogen lights. It can be rotated to illuminate specific areas or objects.
</details>

<details>
  <summary><b>Q: What is unique about a Rectangle Area Light?</b></summary>
  A: Instead of emanating from a point, the Rectangle Area Light emits from an entire rectangular surface, making it ideal for simulating office lighting or larger light sources.
</details>

### Global Lighting Setup

<details>
  <summary><b>Q: What is a Directional Light and why is its position irrelevant?</b></summary>
  A: A Directional Light (commonly used as sunlight) emits parallel rays of light from an infinitely far distance. Its position doesn't matter because the light rays are parallel, only the rotation affects the lighting angle.
</details>

<details>
  <summary><b>Q: What is a Skylight and how does it work?</b></summary>
  A: A Skylight captures distant light in the level and applies it to the scene as ambient light. It provides soft, even illumination from all directions.
</details>

<details>
  <summary><b>Q: What is a Sky Sphere and how does it work with Directional Light?</b></summary>
  A: A Sky Sphere is a massive sphere that simulates the distant sky, clouds, and sun. When linked with a Directional Light, the sky sphere's appearance updates to match the sun's angle, creating physically accurate lighting.
</details>

### Lighting Setup Process

<details>
  <summary><b>Q: What are the three main components needed for a complete global lighting setup?</b></summary>
  A: Sky Sphere, Directional Light, and Skylight
</details>

<details>
  <summary><b>Q: How do you link a Directional Light with a Sky Sphere?</b></summary>
  A: In the Sky Sphere blueprint's details pane, you can select the Directional Light actor to link them together, allowing the sky to update based on the sun's position.
</details>

<details>
  <summary><b>Q: What is the purpose of the "Recapture Scene" function in a Skylight?</b></summary>
  A: The Recapture function updates the Skylight to represent the current atmospheric conditions and lighting from the Sky Sphere, ensuring accurate ambient lighting in the scene.
</details>

### Practical Tips

<details>
  <summary><b>Q: Why might you want to adjust the Directional Light's angle?</b></summary>
  A: To create different moods or times of day in your scene. A higher angle creates midday lighting, while a lower angle can simulate sunrise, sunset, or twilight.
</details>

<details>
  <summary><b>Q: What should you do if the Sky Sphere's appearance doesn't update after changing the Directional Light's angle?</b></summary>
  A: Use the "Refresh Material" function in the BP Sky actor to redraw the sky and update its appearance to match the new sun position.
</details>