# KISS-ICP Configuration Files

This directory contains configuration files for different sensor setups.

## Available Configurations

- `avia.env` - Configuration for Livox AVIA scanner (default for MandEye datasets)

## Configuration Variables

| Variable | Description | Example |
|----------|-------------|---------|
| `INPUT_TOPIC` | ROS topic for input point cloud | `/livox/pointcloud` |
| `OUTPUT_DIR` | Output directory name for results | `results-kiss-icp` |
| `RECORD_TOPICS` | Topics to record from KISS-ICP | `/kiss/local_map /kiss/odometry` |

## Usage

Configs are automatically loaded by `run_benchmark.sh`:

```bash
./run_benchmark.sh avia /path/to/data/
```
