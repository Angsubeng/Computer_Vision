# Project Overview

## "Chart to Text"

The "Chart to Text" project aims to extract text from chart images to make them interpretable. It involves acquiring original Excel data, captions, and titles from Statista, translating them from English to Korean, generating charts using plotly based on the Korean data, and labeling and classifying the generated chart images.

### Data Collection and Translation
1. **Download**: Obtain Excel data, captions, and titles provided by Statista.
2. **Translation**: Translate English files into Korean using methods like Papago crawling, googletrans, or Papago API.

### Chart Generation
1. **Execution**: Run `chart_generator.ipynb` to generate charts with plotly using Korean data, captions, and titles.
2. **Naming**: Save generated chart images with filenames in the format 'data_number_chart_type_chart_direction'.

### Labeling
1. **Processing**: Execute `chart_labeling.ipynb` to apply labeling to generated chart image filenames.
2. **Consistency**: Ensure consistency by applying the same labels to data, captions, and title files.

### Chart Classification
1. **Execution**: Run `chart_classification.ipynb` to classify generated files based on chart types.
2. **Model**: Utilize a pre-trained ResNet50 model trained on ImageNet, employing techniques like data augmentation and early stopping to prevent overfitting.

If further assistance or clarification is needed, feel free to ask.
