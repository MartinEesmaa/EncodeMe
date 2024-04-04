# EncodeMe (by Martin Eesmaa)

EncodeMe is a video media encoder of multi edition. This tool can bring of all encoders & decoders using FFmpeg and external others too with multi platform operating systems.

Operating systems:
Windows, Mac, Linux & FreeBSD (QT C++, Imgui C++, Python, or other programming language)

Android (Kotlin or/and Java)

iOS (Swift)

WebAssembly (TypeScript or Javascript)

CLI (Batchfile, shell script, Python or other programming language)

For using CLI, almost all supported OS can handle in terminal.

Some operating systems can handle all external tools, but it is limited available of some external tools like in mobile and old operating systems.

Also this is construction experimental working on this project since 30th March 2024.

# To-do lists to make release

- CLI
- GUI
- Design of GUI applications
- UV transmissions
- Animations
- Icons
- Detect any fakes
- Optimizations
- Scores of calculation tools
- External tools

# Detect any fakes

The tool uses to detect any media files when using "Detect fake" tab for fake audio bits, audio channels, sample rate, frame per second and video size.

- Duplicated frames must be reencoded to deduplicate video of frames. **It's experimental.**

- Fake video size may be upscaled, needs to be manually check after resized video by human. **It's experimental.**

- Detects fake pixel format for example the original Y4M file is pixel format of 8 bit and upsampled to 10-bit file. 10-bit Y4M file to 8-bit Y4M is match checksum using FFmpeg MD5 format are same video without loss.

- Audio bits & fake audio channels can detect when fake original like 32-bit than original 16-bit or 24-bit.

- Fake audio sample rate of upsampled have to be done on SoX resampler to get back best high quality.

- Check if the audio is lossless or not with cutoff.

# Optimizations

Optimize can be done using FFmpeg to minimize file size without loss quality such as like Matroska, Windows Media and Audio Video Interleave, but stream copy.

# Scores of calculation tools

Video: VMAF from Netflix

Audio: VISQOL from Google

For VISQOL, the maximum range of Audio mode is 4.7321 and needs to be resampled 48khz. For speech mode, it is maximum of range 5 and targets 16khz.

# External tools

External tools are welcome to implement to our tool, includes improvement:

- a52dec (AC3 decoder)
- aften (AC3 encoder)
- AMR-WB+
- Atrac1 & Atrac3 (encoder)
- AudioDec
- AVS3 encoder
- Exhale USAC encoder
- Bonk audio (encoder)
- Encodec
- Enhanced Voice Services
- FAAC & FAAD2 (encoder and decoder)
- FLAC (external)
- FLACCID (best to minimize FLAC audio of encoder)
- FLACCL (CUDA Flac Encoder)
- Flake (Fast Flac Encoder)
- Lagarith (encoder)
- LC3 Google
- LC3plus
- Lyra Google
- MOI (My Optimized IMA-ADPCM)
- Monkey's Audio (encoder, but decode more than stereo channels)
- MP1 (Uzura)
- MPEG-4 ALS
- MPEG-5
- MPEG-H Encoder (Ittiam Systems)
- MPEG-H Decoder (Fraunhofer IIS)
- Musepack
- NIHAV Encoders
- Nintendo DSP-ADPCM
- Nintendo THP
- Quite OK Audio (encoder)
- Sac (state-of-the-art codec lossless)
- WavPack (external)
- More tools lists will come later...

# About this program

This program was created and founded by Martin Eesmaa.