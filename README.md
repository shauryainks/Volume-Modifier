<h1 align="center">Volume Modifier for WAV Files</h1>

This C program is a simple utility designed to modify the volume of audio files in WAV format. It takes three command-line arguments: the input audio file name (`input.wav`), the output audio file name (`output.wav`), and a scaling factor.

## Usage

```bash
./volume input.wav output.wav factor
```

- `input.wav`: The input WAV file to be processed.
- `output.wav`: The output WAV file where the modified audio will be saved.
- `factor`: A floating-point number representing the scaling factor to adjust the volume.

## Instructions

1. Compile the program using a C compiler. For example:

   ```bash
   gcc volume.c -o volume
   ```

2. Run the compiled program with the appropriate command-line arguments:

   ```bash
   ./volume input.wav output.wav factor
   ```

3. Check the specified output file (`output.wav`) for the modified audio.

## Notes

- The program assumes a standard WAV file format with a header size of 44 bytes. This may not be suitable for all WAV files, and additional adjustments may be needed for non-standard formats.

- The scaling operation involves multiplying each 16-bit audio sample by the specified factor. Ensure that the scaling factor avoids distortion and clipping by keeping the resulting values within the valid range for 16-bit audio samples (`-32768` to `32767`).

- Error messages are provided in case of incorrect command-line arguments or file-related issues.


