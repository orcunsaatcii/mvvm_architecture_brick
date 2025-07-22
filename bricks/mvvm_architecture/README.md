# MVVM Architecture Brick

A production-ready project template following the MVVM (Model-View-ViewModel) architecture, designed to quickly bootstrap scalable and maintainable Flutter projects. This brick provides a clear separation of concerns, a modular structure, and the best industry practices.

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
    flutter create my_app
    ```

3.  **Make the Brick**:
    ```sh
    mason make mvvm_architecture
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

## About the Template
- **core/**: Contains all reusable logic, services, and utilities shared across features.
- **feature/**: Each feature is self-contained, with its own views and view models.
- **Extensible**: Add new features by creating new modules under `feature/`.

## Contributing
Feel free to open issues or submit pull requests to improve this template!

---
[1]: https://github.com/orcunsaatcii/mvvm_architecture_brick
