# Image Processing Pipeline

## Overview
This project is building an automation flow to processes and categorize images uploaded automatically to Google Cloud Storage once user upload their picture using Cloud Function. \
The image metadata is stored in Google Cloud Firestore as a documentation and notifications are sent via Google Cloud Pub/Sub to the user for the user experience.

## Setup Instructions

1. Clone the repository:
    ```sh
    git clone https://github.com/your-repo/image-processing-pipeline.git
    cd image-processing-pipeline
    ```

2. Build the Docker image:
    ```sh
    docker build -t image-processor .
    ```

3. Run the Docker container:
    ```sh
    docker run -p 8080:8080 image-processor
    ```

4. Upload images to the Google Cloud Storage bucket and process them by sending a POST request to the `/process_image` endpoint.

## Configuration
Update `config.py` with your Google Cloud project details.
