# Ubuntu-Inspired Image Fetcher

![Ubuntu Logo](https://upload.wikimedia.org/wikipedia/commons/4/4e/Ubuntu_logo_transparent_1.svg)

## The Wisdom of Ubuntu: "I am because we are."

In the spirit of **Ubuntu**, this project is a practical embodiment of its core principles. It emphasizes **community** by connecting to the global network, shows **respect** by gracefully handling potential errors, and promotes **sharing** by organizing fetched resources for easy access and appreciation.

This Python script, `fetch_image.py`, serves as a simple command-line tool to download an image from a given URL and save it to a dedicated directory.

## Features

- **Prompts** the user for a valid image URL.
- **Creates** a `Fetched_Images` directory to organize downloads.
- **Downloads** images using the `requests` library.
- **Handles errors gracefully** for invalid URLs or network issues.
- **Saves** the image with a generated or extracted filename.

## Requirements

Before running the script, ensure you have Python 3 and the `requests` library installed.

```bash
pip install requests
How to Use

    Clone the repository to your local machine:
    Bash

git clone [https://github.com/YourUsername/Ubuntu_Requests.git](https://github.com/YourUsername/Ubuntu_Requests.git)

Navigate into the project directory:
Bash

cd Ubuntu_Requests

Run the script from your terminal:
Bash

    python fetch_image.py

    Enter the URL of the image you want to download when prompted. For example: https://images.unsplash.com/photo-1517849186638-34812a382d67

The image will be saved inside the newly created Fetched_Images directory.

Code Explanation

    requests: This library is used for making HTTP requests to download the image.

    os.makedirs(exist_ok=True): This command ensures the Fetched_Images directory is created only if it doesn't already exist, preventing errors on subsequent runs.

    response.raise_for_status(): This method from the requests library is a simple yet powerful way to check for HTTP errors (like 404 or 500) and raise an exception if one occurs. This is a core part of the "respectful" error handling.

    os.path.basename(urlparse(url).path): This snippet helps to intelligently extract the filename from the URL, providing a clean name for the downloaded file.

Principles Implemented

Principle	Implementation
Community	The program connects to the wider web community to access shared resources.
Respect	It handles errors without crashing, providing a polite message if a connection fails.
Sharing	It organizes fetched images in a clear directory for future use and sharing.
Practicality	It's a useful tool for a common task—downloading and organizing images.

License

This project is open-source and available under the MIT License.

Contributing

Contributions are welcome! If you have suggestions for improvement, please open an issue or submit a pull request.
