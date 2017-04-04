# pdf2datev
Docker image to convert multi-page PDF to monochrome multi-page TIFF for DATEV upload

To convert all PDFs in the current directory and all sub-directories just run:

    docker run --name pdf2datev -v "${PWD}:/images" --rm -it codemonauts/pdf2datev /usr/local/bin/pdf2datev
    
