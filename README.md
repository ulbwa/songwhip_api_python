# [SongWhip](https://songwhip.com) API Wrapper

[![Python 3.10](https://img.shields.io/badge/python-^3.10-blue.svg)](https://www.python.org/downloads/release/python-3100/)
[![MIT License](https://img.shields.io/badge/license-MIT-green.svg)](https://mit-license.org/)

A fast and asynchronous wrapper for the SongWhip API written in Python.

API Documentation: [songwhip.com](https://songwhip.com/faq)

## Installation

```bash
pip3 install git+https://github.com/ulbwa/songwhip_api_python
```
or
```bash
poetry add git+https://github.com/ulbwa/songwhip_api_python
```

## Usage example

```python
import asyncio

from songwhip_api import SongWhip

songwhip = SongWhip()


async def main():
    links = await songwhip.private_request("https://open.spotify.com/album/57zNKp8j0mG1rNtbEVkLMV?si=kWUYHUedRj-vGhGncJD2cw")
    print(links)

asyncio.run(main())
```

