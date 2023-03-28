# Dart Image Converter

[![GitHub release](https://img.shields.io/github/release/jsilverdev/dart_image_converter?include_prereleases=&sort=semver&color=blue)](https://github.com/jsilverdev/dart_image_converter/releases/)
[![License](https://img.shields.io/badge/License-MIT-blue)](#license)
[![issues - dart_image_converter](https://img.shields.io/github/issues/jsilverdev/dart_image_converter)](https://github.com/jsilverdev/dart_image_converter/issues)
![GitHub commits since latest release (by date)](https://img.shields.io/github/commits-since/jsilverdev/dart_image_converter/latest)

A command-line application to transform images and PDF's to resized jpg's images built with Dart

## Features

- Run without need to install dart (compiled files)
- Cross platform (Windows, Linux)
- Easily customizable
- Support many formats: (jpg, png, gif, bmp, tiff, ico, webp, psd, pdf)

## Environment Variables

To run this project, you will need to add the following environment variables to your .env file

`IMAGES_PATH` Required

`WIDTH` Optional. Default value 400 (always in px)

`HEIGHT` Optional. Default value 400 (always in px)

`SEARCH_TERM` Optional. Default value "logo"

`PREFIX_FILE` Optional. Define the prefix name for each generated file. Default is empty

`SKIP_FILES` Optional. Skip or override files. Default to false

`RESULTS_FOLDER` Optional. Folder inside the IMAGES_PATH where the generated images were saved. Default value "results"

## Run Locally

Clone the project

```bash
  git clone https://github.com/jsilverdev/dart_image_converter.git
```

Go to the project directory

```bash
  cd dart_image_converter
```

Install dependencies

```bash
  dart pub get
```

Create .env from the .env.example

```bash
  cp .env.example .env
```

Configure the `IMAGES_PATH` in the .env file

```dotenv
  IMAGES_PATH="path/to/images_path"
```

Start the cli app

```bash
  dart run bin/main.dart
```

## Running Tests

To run tests, run the following command

```bash
  dart test
```

## Run compiled files

### Windows
- Previously configure the .env file and the simply click in the `run_win-x64` file


## Roadmap

- Functionality for upload to GCP