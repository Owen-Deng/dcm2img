# dcm2img
A dcm to image converter based on [DCMTK](https://github.com/DCMTK/dcmtk)'s dcmj2pnm.

- Added JPEG 2000 support by [fmjpeg2koj](https://github.com/DraconPern/fmjpeg2koj). The official JPEG 2000 support is not freely available. This can be an alternative.
- Automatically apply VOI window if exists to avoid images with strange color.

# limitations
- This tool does not support YBR_RCT and YBR_ICT due to limitations of DCMTK.
