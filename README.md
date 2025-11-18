# Resume

This repository contains the LaTeX source code for my resumes.

## Usage

### Building with Docker

You can build the PDF using the provided Docker container to avoid installing LaTeX locally.

1.  **Build the image:**

    ```sh
    docker build -t latex .
    ```

2.  **Build the resumes:**

    ```sh
    # Build fto.pdf
    docker run --rm -i -v "$PWD":/data latex pdflatex fto.tex

    # Build jenny.pdf
    docker run --rm -i -v "$PWD":/data latex pdflatex jenny.tex
    ```

## Output

![Resume Screenshot](/resume_preview.png)
