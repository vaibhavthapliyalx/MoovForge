# 🛠️ MoovForge

MoovForge is a commercial-grade, cross-platform CLI tool for repairing corrupted `.mov`, `.mp4`, and similar video files. It mimics functionality from tools like Remo Repair, featuring atom parsing, moov atom recovery, FFmpeg fallback, and more.

## ✅ Features

- Repair MOV/MP4 files with missing or damaged `moov` atoms
- FFmpeg-based stream fixing fallback
- CLI loading animations and clean UX
- Fully cross-platform (Windows, macOS, Linux)
- Future-ready: includes stubs for GUI (Next.js or Electron)
- Modular, extensible, production-grade codebase

## 🚀 Getting Started

### Installation

You need Python 3.8+ and FFmpeg installed.

Install dependencies (if added later):

```bash
pip install -r requirements.txt
```

### Install FFmpeg (if not installed)

macOS:

```bash
brew install ffmpeg
```

Linux:

```bash
sudo apt install ffmpeg
```

Windows:

Download and extract from: https://ffmpeg.org/download.html

### Usage

```bash
python cli/main.py <input_file> <output_file> --verbose
```

Example:

```bash
python cli/main.py broken.mov fixed.mov --verbose
```

## 📁 Structure

- `cli/` – CLI interface logic
- `core/` – Core repair engine, parser, FFmpeg wrapper
- `tests/` – Simple test cases
- `docs/` – Release notes and documentation
- `scripts/` – Helper install scripts (e.g., FFmpeg)

## ✨ Future Roadmap

- [ ] GUI with Next.js or Electron
- [ ] AI-enhanced content recovery
- [ ] Batch processing support

MIT License.
