# EICAR Test Project

This project contains the EICAR standard antivirus test file and a simple web interface to download it.

## What is EICAR?

The EICAR test file is a standard test file developed by the European Institute for Computer Antivirus Research to safely test antivirus software without using actual malware. When detected, antivirus software should react as if it found a virus, although the file is completely harmless.

## Usage

### Running locally

Simply open the `src/index.html` file in a web browser.

### Running with Docker

```bash
# Build the Docker image
docker build -t eicar-test .

# Run the container
docker run -p 8080:80 eicar-test
```

Then visit http://localhost:8080 in your web browser.

## Warning

This project contains the EICAR test file which will trigger antivirus alerts. This is expected behavior and demonstrates that your antivirus software is working correctly.