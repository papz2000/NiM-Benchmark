# NiM-Benchmark

This is a sample dataset, and we plan to release the full benchmark in the future.

## Overview
This JSON file stores structured data for document-based question answering, mapping questions to answers along with relevant image references.

## JSON Structure
Each entry follows this format:

```json
{
    "question": "<Question text>",
    "answer": "<Answer text>",
    "category": "<Category type>",
    "Image_list": ["<Image path 1>", "<Image path 2>"],
    "Ground truth page": "<Relevant image path>"
}
```

### Fields
- **question**: The question related to the document.
- **answer**: The extracted answer.
- **category**: The type of document-based QA task.
- **Image_list**: Paths to images containing relevant information.
- **Ground truth page**: The main document image verifying the answer.

## Usage
1. **Parsing JSON**: Load and process using JSON-compatible languages.
2. **Querying Answers**: Filter by "question" to retrieve corresponding answers.
3. **Document Processing**: Use paths to locate and analyze relevant document images.

## Notes
- Ensure document image paths are accessible.
- Extend fields as needed for additional document-based QA tasks.
