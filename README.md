# PDFImagify

> A simple PDF to image converter

## Requirements

You can install these with pip

- Flask==1.1.2
- pdf2image==1.14.0
- Pillow==8.1.2

## Usage

### Standalone mode

Call `run.py -i path/to/pdf` in your console

#### Available arguments

- --input (-i): input file or directory (required)
- --output (-o): output directory
- --format (-f): output format
- --lossless (-l): lossless conversion
- --prefix (-p): prefix for output file(s)
- --singlepage (-s): get only the first page from input file(s)
- --width (-w): output file's width

### Server mode

Run `python app.py` in your console or use Gunicorn ([eg. deploy on Heroku](https://devcenter.heroku.com/articles/python-gunicorn)), then call server URL like `http://server?pdf=url/to/pdf`
