# nf-hello-genomics

Welcome to the **nf-hello-world** repository! This is a demonstration pipeline built using [Nextflow](https://www.nextflow.io/), designed to showcase a basic 'hello world' workflow. The pipeline is ideal for demonstrating how to handle input and output files via channels and pass them between processes effectively.

## Overview

The **nf-hello-world** pipeline simply takes a set of greetings, upper cases them, and prints the output to file. It comes with test data located in [./data](./data/) that should run in seconds, allowing you to demonstrate the pipeline quickly. No custom software is required.

## Getting Started

If you are following the hello-nextflow series on https://training.nextflow.io/, you will create a similar version of this pipeline. 

### Prerequisites

To run this pipeline locally, you need to have the following software installed:

- [Nextflow](https://www.nextflow.io/)

### Running the Pipeline

To run the pipeline, use the following command:

```bash
nextflow run seqeralabs/nf-hello-world -profile demo
```

If you wish you can manually supply your own parameters using command line options. These are the defaults specified from the root of the repository:

```bash
nextflow run seqeralabs/nf-hello-genomics \
    --input_file "./data/greetings.csv"
```

This will run the pipeline using the supplied greetings.

#### Parameters

The pipeline allows for the following input parameters:

- `--input_file`: A file containing a comma-separated list of greetings.

Example of running the pipeline:

```bash
nextflow run seqeralabs/nf-hello-world \
    --input_file "./data/greetings.csv"
```

### Advanced Usage

For more advanced usage, such as customizing the workflow, modifying the process definitions, or integrating additional tools, you can edit the `main.nf` file or create custom configurations.

## Credits & Copyright

All training material was originally written by [Seqera](https://seqera.io) but has been made open-source ([CC BY-NC-ND](https://creativecommons.org/licenses/by-nc-nd/4.0/)) for the community.

<a rel="license" href="http://creativecommons.org/licenses/by-nc-nd/4.0/"><img alt="Creative Commons License" src="docs/assets/img/cc_by-nc-nd.svg" /></a>

> Copyright 2020-2023, Seqera. All examples and descriptions are licensed under the <a rel="license" href="http://creativecommons.org/licenses/by-nc-nd/4.0/">Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License</a>.
