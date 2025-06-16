# Traceable

As your project increases in scope so does the complexity of your Product Requirements Document (PRD). 
Traceable is a command line utility for organizing your project's requirements and creating your PRD.

## Installation

```sh
$ brew install techcorrectco/traceable
```

## Usage

After installation you can start Traceable by typing `traceable` in the top-level of a project directory. If Traceable finds a `traceable.json` in the current directory it will load it. If not, it will create one with a single default requirement.

<img width="1536" alt="on-start" src="https://github.com/user-attachments/assets/55b3a3d4-a86e-4169-9f73-c6f4a3645621" />

Pressing `e` with a requirement selected will create a temporary file, populated with the contents of the requirement, and open the temporary file with the editor defined by `$EDITOR`. If `$EDITOR` is undefined, the temporay file will be opened with `nano`.

<img width="1536" alt="on-edit" src="https://github.com/user-attachments/assets/1445bbac-4d16-4178-8e55-9495922da2ad" />

Pressing `n` will create a new sibling requirement and select it. You can navigate sibling requirements by pressing the `up` and `down` arrows.

<img width="1536" alt="new" src="https://github.com/user-attachments/assets/2e9d4c9c-8e34-4ddb-9220-2dd91d0128ab" />

Pressing `c` will create a new child requirement of the currently selected requirement. You can navigate from child to parent by pressing `<`. You can navigate from parent to child by pressing `>`.

<img width="1536" alt="new-child" src="https://github.com/user-attachments/assets/1b136b9a-213a-4ed7-bbae-1c9be3b27f37" />

When you ready to export all your requirements to a PRD, press `x`. A file named `PRD.md` will be created in the current directory.

# Reporting Issues

Open a issue in this repository or send an email to [mark@technicallycorrect.company](mailto:mark@technicallycorrect.company).
