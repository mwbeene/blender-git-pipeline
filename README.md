# Blender Git Pipeline
This repository shows how Blender can be used with Github to allow for synchronous work between team members.

## Folder Structure

### Materials
This folder contains .blend files that contain common materials that will be shared across different models. The textures subfolder contains any texture dependencies.

### Models
The models folder contains subfolders for individual assets. Each subfolder contains the .blend and any unique dependencies and resources. These models may link to materials in the in the materials folder if they use any common materials.

### Sets
Sets are .blend files that contain links to multiple models that need to be exported together into a project-ready format. If multiple models share the same material from the materials folder, their dependencies will only be included once to prevent duplicated data. The exports folder contains gltf and/or glb files ready for your application.

## Dependencies
The Blender files were created in Blender 2.92.0

## License

This project is licensed under the MIT License - see the LICENSE.md file for details