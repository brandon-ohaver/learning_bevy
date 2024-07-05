# This is my first attempt at making a Bevy project. I am using this project as both a learning opportunity for game development, but also as a sort of template for future projects as I work on getting better at my current skills

## NOTES
### What is the App Struct
#### App is a struct made up of three fields: world, schedule, and runner. The `world` filed stores all of the game's data, the `scedule` holds the systems that operatre on this data(and the order in which they do so) and the `runner` interprets the schedule to control the broad execution strategy.

#### Generally, operations will be done at a more granular level than these basic primitives: controlling data in terms of specifici resources or components and adding systems to an existing schedule. To do so, customize the `App` by chaining its methods with the `builder pattern`. The most basic tools are as follows:

#### 1. Initializing resources in the `World` to store globally available data that we only need a single copy of.

#### 2. Adding systems to our `Schedule`, which can read and modify resources and our entities' components, according to our game logic.

#### 3. Importing other blocks of `App` -modifying code using `Plugins`

#### Now to move on to Bevy ECS!
