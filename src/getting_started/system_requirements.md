# System Requirements

## Storage

The system requires roughly 3TB of storage. We need to store the full blockchain history (approximately 280GB), bitgodine parsed history (approximately 2TB), bitgodine transaction security analysis (approximately 250GB), tags and clusters (approximately 90GB).

If you don't need all the storage described above, you can save space avoiding some of the system services.

## Memory

Memory usage is really high and we provisioned a server with 128GB of RAM, that we suggest as minimum requirement. In the future, memory usage could be improved and this requirement could decrease.

## CPU

In order to benefit from concurrency and parallelism we mounted a 10 core Xeon CPU. The main benefit from more processor power is sync time starting from scratch and analysis time.
