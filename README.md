# Technician

Simple gem to wrap a script to process OCR output from a newspaper project.

## Installation

- git clone the project
- bundle install
- gem build technician.gemspec
- gem install 

## Usage

```
$ technician /directory/for/processing/
```

## Directories

Initial directory should look something like this for two issues processed at the same time.

```
/directory/for/processing/
└── output
    ├── Export results 1.10.2014 12.10.36 PM
    │   ├── technician-v48n8-1963-10-02_0001.txt
    │   ├── technician-v48n8-1963-10-02_0002.txt
    │   ├── technician-v48n8-1963-10-02_0003.txt
    │   ├── technician-v48n8-1963-10-02_0004.txt
    │   ├── technician-v48n9-1963-10-03_0001.txt
    │   ├── technician-v48n9-1963-10-03_0002.txt
    │   ├── technician-v48n9-1963-10-03_0003.txt
    │   └── technician-v48n9-1963-10-03_0004.txt
    └── Export results 1.10.2014 12.11.30 PM
        ├── technician-v48n8-1963-10-02_0001.pdf
        ├── technician-v48n8-1963-10-02_0002.pdf
        ├── technician-v48n8-1963-10-02_0003.pdf
        ├── technician-v48n8-1963-10-02_0004.pdf
        ├── technician-v48n9-1963-10-03_0001.pdf
        ├── technician-v48n9-1963-10-03_0002.pdf
        ├── technician-v48n9-1963-10-03_0003.pdf
        └── technician-v48n9-1963-10-03_0004.pdf

```

During processing two other directories will be created.

1. /directory/for/processing/tmp/ can be blown away.
2. /directory/for/processing/final/ are the versions that can be uploaded.