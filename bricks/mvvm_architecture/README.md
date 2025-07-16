# MVVM Architecture Brick

A production-ready project template following the MVVM (Model-View-ViewModel) architecture, designed to quickly bootstrap scalable and maintainable Flutter projects. This brick provides a clear separation of concerns, a modular structure, and the best industry practices.

## Features
- **Solid MVVM Architecture**: A clear separation between the UI (View), business logic (ViewModel), and data layers.
- **Scalable Folder Structure**: The `core` and `feature` modules make it easy for the project to grow.
- **Dynamic Project Setup**: Creates a project customized for you by taking values like project name, organization name, and API address.
- **Ready-to-use Network Layer**: A `Dio`-based, centrally configured network client that includes logging and error handling.
- **Lightweight State Management**: A starting state management solution with Flutter's own `ChangeNotifier`, requiring no external packages.
- **Base Classes**: A `BaseViewModel` that contains common behaviors for all ViewModels.


## How to Use

1.  **Install Mason CLI** (if not already installed):
    ```sh
    dart pub global activate mason_cli
    ```

2.  **Add the Brick from BrickHub**:
    ```sh
    mason add -g mvvm_architecture
    ```
    *Or to add it locally:*
    ```sh
    mason add mvvm_architecture --path /path/to/your/brick
    ```

3.  **Create Your Project**:
    ```sh
    mason make mvvm_architecture -o ./my_awesome_app
    ```


## Detailed Folder Structure

The `lib` folder of the generated project forms the heart of the application and is structured as follows:

```
lib/
├── core/           # Reusable core modules (network, state, utils, etc.)
│   ├── common/     # Common base classes and interfaces
│   ├── config/     # App configuration (localization etc.)
│   ├── models/     # Data models
│   ├── network/    # API and network management
│   ├── routes/     # App routing
│   ├── service/    # Core services
│   ├── state/      # State management
│   └── utils/      # Utilities (constants, extensions, helpers)
└── feature/        # App features (modular)
    ├── auth/       # Authentication feature module
    └── home/       # Home feature module
        ├── view/           # UI widgets and screens
        │   ├── mixin/      # View mixins
        │   └── widget/     # Custom widgets
        └── view_model/     # ViewModel for business logic
```

## Usage
1. **Install Mason** (if you haven't):
   ```sh
   dart pub global activate mason_cli
   ```
2. **Add this brick**:
   ```sh
   mason add mvvm_architecture --source=brichub
   ```
3. **Generate your project**:
   ```sh
   mason make mvvm_architecture
   ```
4. **Start building!**

## About the Template
- **core/**: Contains all reusable logic, services, and utilities shared across features.
- **feature/**: Each feature is self-contained, with its own views and view models.
- **Extensible**: Add new features by creating new modules under `feature/`.

## Contributing
Feel free to open issues or submit pull requests to improve this template!

---
[1]: https://github.com/orcunsaatcii
