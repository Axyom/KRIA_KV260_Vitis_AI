# KRIA_KV260_Vitis_AI

This repository documents and tracks the creation of a complete Vitis AI system for the Kria KV260 board, built from the ground up using the Vivado design flow.

## Objective

The goal is to construct a working hardware and software platform for Vitis AI by directly integrating the required components into a custom Vivado block design. This includes full control over hardware integration, boot flow, and runtime deployment.

## Key Notes

- The DPU (Deep Learning Processing Unit) is not included in the standard Vivado IP catalog.
- To use the DPU, it must be manually added to the root of the project directory.
- The DPU folder is excluded from version control (`.gitignore`), and must be re-added manually after cloning.
- All block designs are exported as `.tcl` scripts to ensure reproducibility.

## Structure

- `*.xpr`: Vivado project file
- `*.srcs/`: HDL sources and block design files
- `*.tcl`: Scripts to recreate the block design and project structure
- `.gitignore`: Excludes all generated and cache files

## Usage

1. Clone the repository
2. Manually place the DPU IP folder in the project root
3. Launch Vivado
4. Source the provided TCL scripts to recreate the design
5. Generate bitstream, export hardware, and proceed to PetaLinux or Vitis steps

## Status

Work in progress.