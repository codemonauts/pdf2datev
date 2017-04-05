# pdf2datev
Docker image to convert multi-page PDF to monochrome multi-page TIFF for DATEV upload

The script first normalizes all filenames to lowercase and removes known problematic chars. After sucessful converting a PDF to a TIFF, the script removes the PDF!

To convert all PDFs in the current directory and all sub-directories just run:

    docker pull codemonauts/pdf2datev
    docker run --name pdf2datev -v "${PWD}:/images" --rm -it codemonauts/pdf2datev /usr/local/bin/pdf2datev
    
