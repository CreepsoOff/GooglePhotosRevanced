# Google Photo Revanced Patched

![GitHub Workflow Status](https://github.com/CreepsoOff/google_photo_revanced/actions/workflows/main.yml/badge.svg) 

## Overview

**Google Photo Revanced Patched** is a GitHub repository that automates the process of downloading the latest APK of Google Photos and the latest releases of ReVanced. Using GitHub Actions, this project compiles these elements into a release, allowing you to easily obtain the patched version of Google Photos.

## Features

- Automatically downloads the latest Google Photos APK.
- Fetches the most recent releases of ReVanced.
- Patches the APK with ReVanced features.
- Creates a release with a version specified in the `version.txt` file.

## Workflow

This project uses GitHub Actions to run the following steps:

1. **Checkout the Repository**: Retrieves the latest code from the repository.
2. **Setup Python**: Installs Python and required dependencies.
3. **Download APKs and ReVanced Files**: Executes a Python script to fetch the necessary files.
4. **Patch Google Photos APK**: Uses `revanced-cli` to patch the downloaded APK.
5. **Create Output Directory**: Prepares a directory for the patched APK.
6. **Move Patched APK**: Places the patched APK in the output directory.
7. **Create a Tag and Release**: Tags the release based on the version specified in `version.txt`.
8. **Publish the Release**: Creates a GitHub release with the patched APK.

## Versioning

To specify the version for each release, create or update the `version.txt` file in the repository. The current format is:


### Coming Soon

- Automated versioning system to generate version names in the format `Google_photo.[Google Photos version].[Patch version]`.

## Installation

To use this project, you need to create a GitHub repository and set up GitHub Actions. Follow these steps:

1. **Fork or Clone this Repository**.
2. **Create a `version.txt` file** at the root of the repository to specify the version.
3. **Enable GitHub Actions** for your repository.

## Usage

Once the workflow is set up, any push to the `master` branch will trigger the automated process, creating a new release with the latest patched APK.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements or suggestions.

## License

This project is licensed under the [GPL 3.0](LICENSE).

## Acknowledgments

- Thanks to the [ReVanced](https://github.com/ReVanced) team for their work on the patching tool.
- Thanks to [APKPure](https://apkpure.com) for providing APK downloads.

