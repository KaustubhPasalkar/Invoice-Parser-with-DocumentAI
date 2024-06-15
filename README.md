## Invoice-Parser-with-DocumentAI
The document provides a comprehensive guide on how to set up and uptrain an Invoice Parser using Google Cloud's Document AI. Here is a breakdown of the content:

Steps to Setup Invoice Parser in Document AI
### 1. Create New Project:
Start by creating a new project in Google Cloud.

### 2. Create a Processor:
In the Google Cloud console, navigate to Document AI and select the Processor Gallery.
Search for Invoice Parser and create a new processor, giving it a name and selecting the closest region.

<img width="752" alt="DocumentAI1" src="https://github.com/KaustubhPasalkar/Invoice-Parser-with-DocumentAI/assets/52817783/5e9788c6-44fc-47c7-96df-1a36dcddd943">

### 3. Create a Cloud Storage Bucket for the Dataset:
Create a new Cloud Storage bucket to store the dataset required for training and testing the processor.

### 4. Import a Sample Document for Manual Labeling:
Import a sample invoice PDF file into your dataset for manual labeling to help the processor identify the entities to extract.
Label the fields in the sample document using the provided tools.

<img width="742" alt="DocumentAI2" src="https://github.com/KaustubhPasalkar/Invoice-Parser-with-DocumentAI/assets/52817783/71c2dbc9-ac5a-4cfc-a09c-c8683a26f9ac">

### 5. Define Processor Schema:
Edit the schema to mark unused labels as inactive and add custom labels if needed before starting the training.

<img width="769" alt="DocumentAI8" src="https://github.com/KaustubhPasalkar/Invoice-Parser-with-DocumentAI/assets/52817783/5669ef57-d814-40c9-bd3a-5fcd229c372f">

### 6. Label a Document:
Annotate the sample document by selecting text and applying labels. Ensure all instances of an entity are annotated correctly.

<img width="745" alt="DocumentAI3" src="https://github.com/KaustubhPasalkar/Invoice-Parser-with-DocumentAI/assets/52817783/43c0a9c1-87a8-4057-be70-8cc2c9b50dda">

### 7. Assign Annotated Document to the Training Set:
Assign the labeled document to the training set to prepare it for training.

### 8. Import Pre-labeled Data to the Training and Test Sets:
Import pre-labeled documents into the training and test sets, ensuring you have enough documents and label instances for effective training.
Optionally, use auto-labeling for new documents if there is an existing deployed processor version.

<img width="751" alt="DocumentAI4" src="https://github.com/KaustubhPasalkar/Invoice-Parser-with-DocumentAI/assets/52817783/fc95d78c-47a8-465e-a898-726c74ba9e44">

### 9. Train the Processor:
Start the training process after setting up the processor with the appropriate data and labels. Training may take several hours.

### 10. Deploy the Processor Version:
Deploy the trained processor version to make it ready for use.

<img width="745" alt="DocumentAI5" src="https://github.com/KaustubhPasalkar/Invoice-Parser-with-DocumentAI/assets/52817783/1585bb3d-861b-4d1d-8f6d-e6a758ec6704">


### 11. Evaluate and Test the Processor:
Evaluate the processor's performance using metrics like F1 score, precision, and recall.
Test the processor with new documents not used in training or testing to validate its performance.

<img width="744" alt="DocumentAI6" src="https://github.com/KaustubhPasalkar/Invoice-Parser-with-DocumentAI/assets/52817783/45b8cc20-7bef-4240-b648-ecf8ba110791">


### 12. Use the Processor:
Manage your custom-trained processor versions and send processing requests to handle entity extraction tasks.

<img width="744" alt="DocumentAI7" src="https://github.com/KaustubhPasalkar/Invoice-Parser-with-DocumentAI/assets/52817783/1223321c-84d4-490e-9c4f-88995808f27b">

## Key Points
### Manual Labeling: 
Manually label a sample document to guide the processor.
### Schema Management: 
Edit and manage the schema to include only relevant labels.
### Training Data: 
Ensure a sufficient number of labeled documents in the training and test sets.
### Training and Deployment: 
Train the processor and deploy the trained version.
### Evaluation: 
Evaluate the processor using various metrics and test it with new data.
### Usage: 
Use and manage the custom-trained processor for processing requests.
