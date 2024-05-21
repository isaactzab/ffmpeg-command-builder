# FFmpeg Command Builder

FFmpeg Command Builder is a library designed to simplify the creation and execution of complex FFmpeg commands. This tool helps streamline multimedia processing tasks by providing dynamic filter support and a user-friendly interface for building FFmpeg commands.

## Features

- **Dynamic Filter Support**: Easily apply various filters such as `negate`, `hflip`, `edgedetect`, `hstack`, `vstack`, and `overlay`.
- **Customizable Commands**: Build and customize FFmpeg commands to fit your specific needs.
- **Ease of Use**: Simplify the process of generating FFmpeg command strings and executing them.
- **Efficient Processing**: Optimize multimedia workflows with a streamlined command generation process.

## Installation

To install FFmpeg Command Builder, clone the repository and install the dependencies:

```bash
git clone https://github.com/yourusername/ffmpeg-command-builder.git
cd ffmpeg-command-builder
npm install

## Example JSON Input

```{
  "in": [
    {"id": "0", "file": "input1.mp4"},
    {"id": "1", "file": "input2.mp4"}
  ],
  "filters": [
    {"filter": "hflip", "in": "0", "out": "a"},
    {"filter": "vstack", "in": ["a", "1"], "out": "b"},
    {"filter": "overlay", "params": {"x": 10, "y": 20}, "in": "b", "out": "c"}
  ],
  "out": "output.mp4"
}
```
