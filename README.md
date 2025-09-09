v# Ubuntu-Inspired Image Fetcher

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
