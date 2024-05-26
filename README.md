```sh
docker build -t latex .
docker run --rm -i -v "$PWD":/data latex pdflatex fto.tex
```

![Resume Screenshot](/resume_preview.png)

