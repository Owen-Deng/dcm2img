# dcm2img
A dcm to image converter based on [DCMTK](https://github.com/DCMTK/dcmtk)'s dcmj2pnm.

- Added JPEG 2000 support by [fmjpeg2koj](https://github.com/DraconPern/fmjpeg2koj). The official JPEG 2000 support is not freely available. This can be an alternative.
- Automatically apply VOI window if existed to avoid images with strange color.

# Dependencies
- sudo apt install libopenjp2-7

# Build by yourself
- sudo apt install cmake build-essential
- build DCMTK by following the official instructions
- build openjpeg following the official instructions
- build dcm2img

# limitations
- This tool does not support YBR_RCT and YBR_ICT due to limitations of DCMTK.

# Useage
See `dcm2img -h`
