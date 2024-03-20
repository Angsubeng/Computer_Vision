**Project Overview:**

"Chart to text" presents a process of extracting text from chart images to transform them into interpretable images. Initially, the original Excel data, captions, and titles from Statista are acquired as files and then translated from English to Korean. Subsequently, in the chart_generator.ipynb file, based on the Korean data, captions, and titles, 4 types of charts (Bar, Line, Pie, Table) are generated using plotly. The generated chart images are saved with filenames in the format 'data_number_chart_type_chart_direction'.

**Execution Steps:**

**Data Collection and Translation:**
1. Download the Excel data, captions, and titles provided by Statista.
2. Translate the English files into Korean. This can be achieved using methods such as Papago crawling, googletrans, or Papago API.

**Chart Generation:**
1. Execute the chart_generator.ipynb file to generate charts using plotly based on Korean data, captions, and titles.
2. The generated chart images are named according to the corresponding data number, chart type, and chart direction.

**Labeling:**
1. Run the chart_labeling.ipynb file to apply labeling to the generated chart image filenames.
2. Ensure consistency by applying the same labels to the data, captions, and title files.

**Chart Classification:**
1. Execute the chart_classification.ipynb file to classify the generated files according to chart types.
2. Utilize a pre-trained ResNet50 model trained on ImageNet, employing techniques such as data augmentation and early stopping to prevent overfitting. 

If you need further assistance or clarification, feel free to ask.
