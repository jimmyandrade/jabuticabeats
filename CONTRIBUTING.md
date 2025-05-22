# Contributing

We welcome contributions to this project! Please follow these guidelines to ensure a smooth development process.

## Development Workflow

[You can add your project's specific development workflow details here, e.g., branching strategy, code style, testing procedures.]

## Managing Dependencies

This project enforces the use of exact versions for all npm dependencies to ensure consistency, stability, and avoid unexpected issues arising from version mismatches or unintended updates.

### Adding New Dependencies

1.  **Configuration for Exact Versions**: The project is configured with an `.npmrc` file containing `save-exact=true`. This means that when you add a new package, npm will automatically save its exact version to `package.json`.

2.  **Installation**: To add a new dependency, simply run:
    ```bash
    npm install <package-name>
    ```
    Or, for a development dependency:
    ```bash
    npm install <package-name> --save-dev
    ```
    You do **not** need to add the `--save-exact` flag manually; the `.npmrc` file handles this.

3.  **Verify `package-lock.json`**: After installing a new dependency, `package.json` and `package-lock.json` will be updated. Please ensure these changes are committed along with your code. The `package-lock.json` file is crucial as it records the exact versions of all dependencies and their sub-dependencies.

4.  **Why Exact Versions?**:
    *   **Reproducibility**: Ensures that every developer and the CI/CD environment installs the exact same version of every package, leading to reproducible builds.
    *   **Stability**: Protects against accidental upgrades to new minor or patch versions that might introduce bugs or breaking changes.
    *   **Clarity**: `package.json` directly reflects the specific versions being used, reducing ambiguity.

### Updating Dependencies

If you need to update a dependency, it should be a deliberate action:

1.  Install the new version specifically:
    ```bash
    npm install <package-name>@<version>
    ```
2.  Test thoroughly after updating.
3.  Commit the updated `package.json` and `package-lock.json` files.

[Add any other contribution guidelines specific to your project below.]
