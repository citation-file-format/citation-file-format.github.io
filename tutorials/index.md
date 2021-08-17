---
title: Citation File Format - Tutorials
---

## Validating `CITATION.cff` files

The Citation File Format provides a [JSON Schema](https://json-schema.org/) file 
([`schema.json`](https://github.com/citation-file-format/citation-file-format/blob/main/schema.json))
that `CITATION.cff` files can be validated against.

### Docker

If you use `docker`, you can validate your `CITATION.cff` file as follows.

1. Build the docker container:
```bash
docker build -t cffvalidator \
https://raw.githubusercontent.com/sdruskat/cff-validator-docker/1.0.0/Dockerfile
```
2. Run the container. Note that you have supply the absolute path to the local `CITATION.cff` file you want to validate with `-v`:
```bash
docker run --rm \
-v </absolute/path/to/your/CITATION.cff>:/cff/CITATION.cff cffvalidator
```

### Python 3

The [Citation File Format README](https://github.com/citation-file-format/citation-file-format#validation-heavy_check_mark)
describes how to validate `CITATION.cff` files in Python 3.

If you want to avoid cloning the Citation File Format repository, as described there, you can also [download the Python script directly](https://github.com/citation-file-format/citation-file-format/blob/main/examples/validator.py). Note that you may still need to install the required Python packages.
