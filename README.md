# Furnilytics Python Library

Official Python client for the Furnilytics API.

Furnilytics provides structured market and industry data for the furniture sector via a simple API.

## Installation

```bash
pip install furnilytics
```
## Authentication

Create an API key in your Furnilytics dashboard and set it as an environment variable:
```bash
export FURNILYTICS_API_KEY="your_api_key"
```
## Quick Start
```python
from furnilytics import Client

client = Client()

data = client.get("furniture/chairs/market_size")
print(data)
```
## Usage

The `get` method follows the structure:

```python
client.get("<topic>/<subtopic>/<dataset>", **params)
```
Example with parameters:
```python
data = client.get(
    "furniture/chairs/market_size",
    country="US",
    year=2024
)
```
## Documentation

Full API documentation, available datasets, and usage guides can be found at:

https://www.furnilytics.com/api/

## Issues and Support

If you encounter a bug or have a feature request, please open an issue in this repository.

For general questions, contact support via the Furnilytics website.

## License

This project is licensed under the MIT License.
