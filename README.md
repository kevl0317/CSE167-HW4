# CSE167HW4-Acceleration Structure

> This page only serves as a guide to our program. No code will be posted here.

# Run the code

> This program will run on Windows computers, Visual Studio 2022 worked for us.
> 1. Open the `.sln` file in the folder
> 2. Enter the `scene.test` file to render in Visual Studio.
> 3. Click the green arrow on the top of Visual Studio, run with `Release` is suggested.
> 4. Then the program will start rendering.

<img src="progress.png">

# Explaination
> We implemented bounding boxes for the acceleration stucture. We first created a cuboid that wraps all objects in the scene, then divide the cuboid into smaller cubes. We also calculated the wrapping cuboid for every triangle and sphere, then found where they are in the scene cuboid. When we have an incoming ray, we now only need to consider the traingles and spheres inside the cuboids intersected along the way, which can be calculated efficiently.

# Results
> After implementing this acceleration structure, we successfully sped up the rending time of `scene7.test` from `30 - 40 minutes` to only `3 minutes`.

> Before Acceleration

<img src="pre-acceleration.png">

> After Acceleration

<img src="post-acceleration.png">


Kevin Liu, Yuan Gao
