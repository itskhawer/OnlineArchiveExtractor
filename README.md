# OnlineArchiveExtractor

**OnlineArchiveExtractor** is a Python-based tool designed to download and extract compressed files directly from URLs to Google Drive using Google Colab. It supports multiple archive formats, including `.zip`, `.rar`, and `.tar`.

## Features

- **File Download**: Downloads files from any URL with progress tracking.
- **Archive Extraction**: Supports `.zip`, `.rar`, and `.tar` formats.
- **Google Drive Integration**: Extracted files are saved directly to a specified folder in Google Drive.
- **Progress Monitoring**: Displays progress bars for downloading and extraction.

## Installation

1. Clone the repository or copy the script to your local environment:
   ```bash
   git clone https://github.com/itskhawer/OnlineArchiveExtractor.git
   ```

2. Install the required Python packages:
   ```bash
   pip install rarfile tqdm requests
   ```

3. Open and run the script in [Google Colab](https://colab.research.google.com/).

## Usage

1. Open the script in Google Colab.
2. Mount your Google Drive:
   ```python
   drive.mount('/content/drive')
   ```
3. Run the script and follow the prompts:
   - Enter the URL of the compressed file.
   - The tool will download the file, extract it, and save the contents to Google Drive.

### Example Workflow

1. Provide the URL of a compressed file (e.g., `https://example.com/sample.zip`).
2. The file will be downloaded and extracted to:
   ```
   /content/drive/My Drive/Extracted/sample
   ```

## Supported Formats

- `.zip`
- `.rar`
- `.tar`, `.tar.gz`, `.tgz`, `.tar.bz2`

## File Structure

- `download_file(url, temp_save_path)`: Downloads files with progress tracking.
- `extract_file(file_path, extract_to)`: Extracts files based on their format.
- `main()`: Orchestrates the download and extraction process.

## Contributing

Contributions are welcome! If you have suggestions or improvements, feel free to fork the repository and submit a pull request.

## Disclaimer

This tool is provided for educational purposes. Please ensure you have the rights to download and extract files from the specified URLs.
