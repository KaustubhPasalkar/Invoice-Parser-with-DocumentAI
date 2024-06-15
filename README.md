## Invoice-Parser-with-DocumentAI
The document provides a comprehensive guide on how to set up and uptrain an Invoice Parser using Google Cloud's Document AI. Here is a breakdown of the content:

Steps to Setup Invoice Parser in Document AI
### 1. Create New Project:

Start by creating a new project in Google Cloud.
Create a Processor:

In the Google Cloud console, navigate to Document AI and select the Processor Gallery.
Search for Invoice Parser and create a new processor, giving it a name and selecting the closest region.
Create a Cloud Storage Bucket for the Dataset:

Create a new Cloud Storage bucket to store the dataset required for training and testing the processor.
Import a Sample Document for Manual Labeling:

Import a sample invoice PDF file into your dataset for manual labeling to help the processor identify the entities to extract.
Label the fields in the sample document using the provided tools.
Define Processor Schema:

Edit the schema to mark unused labels as inactive and add custom labels if needed before starting the training.
Label a Document:

Annotate the sample document by selecting text and applying labels. Ensure all instances of an entity are annotated correctly.
Assign Annotated Document to the Training Set:

Assign the labeled document to the training set to prepare it for training.
Import Pre-labeled Data to the Training and Test Sets:

Import pre-labeled documents into the training and test sets, ensuring you have enough documents and label instances for effective training.
Optionally, use auto-labeling for new documents if there is an existing deployed processor version.
Train the Processor:

Start the training process after setting up the processor with the appropriate data and labels. Training may take several hours.
Deploy the Processor Version:

Deploy the trained processor version to make it ready for use.
Evaluate and Test the Processor:

Evaluate the processor's performance using metrics like F1 score, precision, and recall.
Test the processor with new documents not used in training or testing to validate its performance.
Use the Processor:

Manage your custom-trained processor versions and send processing requests to handle entity extraction tasks.
Key Points
Manual Labeling: Manually label a sample document to guide the processor.
Schema Management: Edit and manage the schema to include only relevant labels.
Training Data: Ensure a sufficient number of labeled documents in the training and test sets.
Training and Deployment: Train the processor and deploy the trained version.
Evaluation: Evaluate the processor using various metrics and test it with new data.
Usage: Use and manage the custom-trained processor for processing requests.
This guide is essential for anyone looking to implement an Invoice Parser with Google Cloud's Document AI, providing a structured approach to setting up, training, and deploying the processor for extracting entities from invoices.
