# BNK
# Stock Report Monitoring System

Monitor stock market reports and receive notifications about updates through a messaging bot.

## Table of Contents

- [Introduction](#introduction)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [Usage](#usage)
- [Functionality](#functionality)
- [Configuration](#configuration)
- [Bot Integration](#bot-integration)
- [Troubleshooting](#troubleshooting)
- [Contributing](#contributing)
- [License](#license)

## Introduction

The Stock Report Monitoring System is a Python script that fetches stock market reports using the DART API and notifies users about new reports through a messaging bot. This system is useful for staying updated with the latest stock market developments and making informed investment decisions.

## Getting Started

Follow these instructions to set up the Stock Report Monitoring System on your local machine.

### Prerequisites

- Python 3.7 or later
- DART API key (obtainable from [DART website](https://dart.fss.or.kr/))
- Required libraries: pandas, datetime, time (install using `pip install pandas`)

### Installation

1. Clone this repository: `git clone https://github.com/yourusername/stock-report-monitoring.git`
2. Navigate to the project directory: `cd stock-report-monitoring`
3. Install required libraries: `pip install -r requirements.txt`

## Usage

To use the Stock Report Monitoring System:

1. Obtain a DART API key from the [DART website](https://dart.fss.or.kr/).
2. Configure the `api_key`, `t_date`, and other settings in the code.
3. Run the script using: `python main.py`

## Functionality

The Stock Report Monitoring System consists of the following functions:

### `get_data()`

Fetches stock market reports using the DART API, converts the data into a DataFrame, and returns it.

### `check_for_updates(previous_data)`

Compares the new data with the previous data, identifies new reports, and sends notifications through a messaging bot.

### `bot_msg(df)`

Constructs and sends bot messages based on the type of report in the new data.

## Configuration

Before running the script, configure the following settings in the `main.py` file:

- `api_key`: Your DART API key.
- `t_date`: The target date for fetching reports.
- Messaging bot settings: Configure messaging bot integration.

## Bot Integration

The script integrates with a messaging bot to send notifications about new reports. Configure your messaging bot credentials and chat IDs for different types of reports in the `bot_msg()` function.

## Troubleshooting

If you encounter issues while using the Stock Report Monitoring System, consider the following steps:

- Check your API key and network connectivity.
- Review the error messages in the terminal for insights.

## Contributing

Contributions to the Stock Report Monitoring System are welcome! To contribute, follow these steps:

1. Fork the repository.
2. Create a new branch: `git checkout -b feature-name`
3. Make your changes and commit them: `git commit -m "Add feature"`
4. Push to the branch: `git push origin feature-name`
5. Create a pull request.

## License

This project is licensed under the [MIT License](LICENSE).
