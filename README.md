# label_parsing_function_demo

This project contains code for parsing and reformatting results from Form Recognizer & Custom Vision. 

## Environment Setup
Before running this project, create a `local.settings.json` file in the root directory. This file needs to have the following entries under the `values` section:

| Key | Value |
|-----|-------|
| AzureWebJobsStorage                 | The connection string to the storage account used by the Functions runtime.  To use the storage emulator, set the value to UseDevelopmentStorage=true |
| FUNCTIONS_WORKER_RUNTIME            | Set this value to `python` as this is a python Function App | 
| UPLOAD_STORAGE_ACCOUNT_URL | Blob storage account URL for the storage account where processed results will be uploaded |
| UPLOAD_STORAGE_ACCOUNT_KEY | Blob storage account key for the storage account where processed results will be uploaded |
| OUTPUT_CONTAINER | Name of the storage container where processed results will be uploaded |