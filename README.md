# Azusa Recipes Helper

This repository, **azusa-recipes-helper**, is a support tool for managing software recipes in [AzusaOS](https://github.com/azusaOS). It simplifies software version tracking, updates, and builds for AzusaOS packages.

## Features

- **Application Database and Recipe Management**  
  A helper script that supports maintaining the application database or recipe.

- **Versioned Application List in Multiple Formats**  
  Outputs lists of applications with version information and sources in:
  - **CSV**: [`VERSIONS.csv`](VERSIONS.csv)
  - **Markdown**: [`VERSIONS.md`](VERSIONS.md)
  - **NVChecker format**: [`NVChecker.toml`](NVChecker.toml)

- **Automatic Version Checking with NVChecker**  
  Templates for [NVChecker](https://github.com/lilydjwg/nvchecker) to track and verify application versions.

## TODO

1. **Automate Version Checks**
   - Set up a cron job or GitHub Action to use NVChecker for version tracking and updates.

2. **Build Automation on Software Update**
   - Configure GitHub Actions and shell scripts to trigger builds on software updates.

3. **Automated AzusaOS ISO Generation**
   - Automate the creation of new AzusaOS ISO files for major updates.

4. **Dockerized GitHub Actions**  
   - Use Docker in GitHub Actions for consistent build and deployment.

### Suggested Enhancements

- **Automated Release Notes**  
  Generate Markdown release notes automatically for each update.

- **Notification System**  
  Send version updates or build completion notifications via Slack or Discord.

- **Build Logs and Artifact Storage**  
  Store logs and build artifacts in a dedicated repository or S3-compatible storage.

## Project Structure

- **[azusa-opensource-recipes](https://github.com/AzusaOS/azusa-opensource-recipes/)** - Open-source application recipes (submodule).
- **LICENSE** - Project license under MIT.
- **NVChecker.toml** - NVChecker configuration for version tracking.
- **VERSIONS.csv** - CSV version list of applications.
- **VERSIONS.md** - Markdown version list of applications.

## Usage

1. **Set Up NVChecker**  
   - Configure `NVChecker.toml` with details for version tracking.

2. **Run Version Check**  
   - Use NVChecker manually, on a schedule, or as a GitHub Action.

3. **Automate Builds and ISO Creation**  
   - Configure GitHub Actions to handle builds and ISO creation when new versions are detected.

## REF

-   [**azusa-opensource-recipes**](https://github.com/AzusaOS/azusa-opensource-recipes/)  
    Recipes for open-source applications used in AzusaOS.
    
-   [**azusa-run**](https://github.com/AzusaOS/azusa-run)  
    Scripts and tools to run various components of AzusaOS.
    
-   [**azusa-docker**](https://github.com/AzusaOS/azusa-docker)  
    Docker configurations and images for AzusaOS applications.
    
-   [**apkg**](https://github.com/AzusaOS/apkg)  
    Package management and automation scripts for AzusaOS applications.
    
## Contributing

We welcome contributions! Please refer to repository issues or suggest new features.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.
