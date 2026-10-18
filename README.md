# VSR GPU Portable Backup

Windows 64-bit portable backup of **Video Subtitle Remover v1.4.0**, rebuilt and repaired for NVIDIA CUDA acceleration.

## Source

This project is based on the following upstream project:

- Upstream: https://github.com/YaoFANGUK/video-subtitle-remover
- Upstream version: Video Subtitle Remover v1.4.0
- Upstream author: YaoFANGUK

This repository is an independent backup of a modified portable build. It is not an official upstream release and is not endorsed by the upstream author. All original project rights remain with the upstream author and contributors.

## What Is Included

- Windows 64-bit portable package.
- PyTorch CUDA build and bundled runtime dependencies.
- No Python, PyTorch, CUDA Toolkit, or FFmpeg installation required.
- GPU inference on compatible NVIDIA graphics cards.
- FFmpeg processes hidden, with no console windows during processing.
- Drag-and-drop hint and drag-and-drop input.
- Output written beside the source video without overwriting it.
- Existing output names are never overwritten; `_no_sub_1`, `_no_sub_2`, and later names are used when needed.
- Audio is converted to AAC 192 kbps and merged into the result.

## Supported Computers

Recommended:

- Windows 11 64-bit.
- NVIDIA RTX 20, 30, 40, or 50 series graphics card.
- A current NVIDIA driver supporting CUDA 12.8.
- At least 4 GB of available GPU memory for the tested configuration.
- Enough free disk space for the source video, temporary files, and the output video.

The package was tested on:

- Windows 64-bit.
- NVIDIA GeForce RTX 3060 Laptop GPU.
- PyTorch 2.11.0 with CUDA 12.8.
- A 362-frame, 832 x 1440 input video.
- Successful processing at 100 percent, with AAC stereo audio in the output.

Not supported directly:

- macOS, Linux, Windows ARM, or 32-bit Windows.
- AMD or Intel graphics as the CUDA inference device.
- Computers without a compatible NVIDIA graphics card.

## Download

Download all release split parts and place them in the same folder. Then open the first part with 7-Zip and extract the complete archive.

Do not run only the launcher from the ZIP. Extract the complete package first, then run:

```text
启动 GPU 版.exe
```

The source file directory must allow creation of new files. Results are written beside the source video as:

```text
video_name_no_sub.mp4
```

## SHA-256

The SHA-256 of the complete portable ZIP is:

```text
BC2F5E0205E51EF417BDE4B858557DCC59372A0A4EDC2E4E2BE4143D733B295B
```

After joining the split parts, verify the reconstructed ZIP against this checksum before extracting it.

## Backup and Distribution

This repository is used as a personal backup and public download location for this portable build. If the upstream project changes or its license requirements change, follow the upstream terms.
