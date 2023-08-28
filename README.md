
# README for Meeting Scheduler Application

Made with DemoGPT for Fall 2023 CS 8395-08

## Introduction

This Streamlit application is designed to assist users in scheduling meetings. It leverages the Langchain library to integrate GPT-3.5 Turbo from OpenAI for generating potential meeting times and confirming them. The application is divided into two main sections:

1. **Availability Input**: Users can enter their availability and preferences for scheduling.
2. **Meeting Time Selection**: Based on the provided availability, the application suggests potential meeting times. Users can then select their preferred time.

## Table of Contents

- [Introduction](#introduction)
- [Installation](#installation)
- [Usage](#usage)
- [Functions](#functions)
  - [meetingScheduler](#meetingscheduler)
  - [meetingConfirmation](#meetingconfirmation)
- [Dependencies](#dependencies)
- [Contributing](#contributing)
- [License](#license)

## Installation

To install the required libraries, use the following:

\```bash
pip install streamlit langchain
\```

## Usage

To run the Streamlit application, navigate to the directory where the code is located and execute:

\```bash
streamlit run <filename>.py
\```

## Functions

### `meetingScheduler`

#### Parameters

- `availability`: A string that contains the user's availability and preferences for scheduling.

#### Return

- `result`: A string that lists potential meeting times based on the provided availability.

#### Description

Uses the Langchain library to prompt a GPT-3.5 Turbo model to generate potential meeting times based on the user's availability.

---

### `meetingConfirmation`

#### Parameters

- `selected_time`: A string that specifies the user's selected meeting time.

#### Return

- `result`: A string confirming the meeting time and providing any additional details or instructions.

#### Description

Uses the Langchain library to prompt a GPT-3.5 Turbo model to confirm the selected meeting time and provide any additional details or instructions.

## Dependencies

- `streamlit`
- `langchain`
- `tempfile`

## Contributing

Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.

---

For more information, please refer to the official documentation of [Langchain](https://langchain.readthedocs.io/) and [Streamlit](https://docs.streamlit.io/).
