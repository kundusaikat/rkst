# RKST (Royal Key Solutions Technologies)

RKST serves as the central repository for managing connected submodules related to various projects under the Royal Key Solutions Technologies umbrella. This repository provides an organized structure for coordinating development across multiple independent repositories, such as `rkst-customer`, `rkst-admin`, and `rkst-api`. 

## Repository Structure

This root repository uses **Git Submodules** to manage child projects. Below is the structure:

```
rkst/
├── rkst-customer/  # Frontend for customers
├── rkst-admin/     # Admin portal
├── rkst-api/       # Backend API services
```

## Getting Started

### Cloning the Repository
When cloning this repository, ensure that you also initialize the submodules:

```bash
git clone --recurse-submodules https://github.com/kundusaikat/rkst.git
```

If you forgot to include `--recurse-submodules`, you can initialize and fetch submodules later:

```bash
git submodule update --init --recursive
```

### Updating Submodules
To pull the latest changes from all submodules, run:

```bash
git submodule update --remote --merge
```

### Adding New Submodules
To add a new submodule to this repository:

1. Run:
   ```bash
   git submodule add <repository-url>
   ```
2. Commit the changes:
   ```bash
   git add .
   git commit -m "Added <submodule-name>"
   git push origin main
   ```

### Removing Submodules
To remove a submodule:

1. Deinitialize the submodule:
   ```bash
   git submodule deinit -f <submodule-name>
   ```
2. Remove the submodule directory:
   ```bash
   rm -rf <submodule-name>
   ```
3. Commit the changes:
   ```bash
   git add .
   git commit -m "Removed <submodule-name>"
   git push origin main
   ```

## Deployment
Each submodule is independently deployed and managed. Ensure you refer to the individual repositories for their respective deployment instructions and configurations.

## Contributing
To contribute to any of the submodules:

1. Navigate to the specific submodule directory.
2. Make your changes.
3. Commit and push changes to the submodule's repository.
   ```bash
   cd <submodule-directory>
   git add .
   git commit -m "Your commit message"
   git push
   ```

## License
This repository is licensed under the [MIT License](LICENSE). Please see the `LICENSE` file for more details.

## Contact
For any inquiries, reach out to **Royal Key Solutions Technologies** at:
- **Email**: support@rkst.in
- **Website**: [www.rkst.in](https://www.rkst.in)