# Rust File Compressor

This Rust project compresses a file using Gzip compression. It takes a source file as input, compresses it, and outputs the compressed file with a specified target name. This project demonstrates basic file handling, buffering, and Gzip compression using Rust.

## Features
- Compresses a specified file using Gzip compression.
- Displays the size of the source and compressed files.
- Shows the time taken to compress the file.

## Dependencies
This project uses the [`flate2`](https://docs.rs/flate2/latest/flate2/) crate for Gzip compression. 

### Cargo.toml
Ensure the following dependency is added to your `Cargo.toml` file:
```toml
[dependencies]
flate2 = "1.0"

Usage
Build the Project: Clone this project and navigate to its directory, then build with Cargo:

bash
Copy code
cargo build --release
Run the Project: After building, run the program with:

bash
Copy code
cargo run --release <source-file> <target-file>
<source-file>: Path to the file you want to compress.
<target-file>: Path where the compressed file will be saved.
Example
bash
Copy code
cargo run --release example.txt example.txt.gz
Code Overview
Arguments: The program expects two command-line arguments: the source file and the target file.
Compression: It reads the source file, compresses it with Gzip, and writes it to the target file.
Timing: It tracks and displays the time taken for the compression process.
Output: Shows the sizes of the original and compressed files for comparison.
Example Output
After running, you might see output like:

python
Copy code
Source len: 1024 bytes
Target len: 256 bytes
Elapsed: 0.1s
License
This project is open-source and available under the MIT License.

This `README.md` provides a clear overview of the project, setup, usage, and example output, making it easy for others to understand and use your project.
