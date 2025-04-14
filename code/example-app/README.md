# Example End to End Flow

## Create Python Environment

1. Create a virtual environment:
   ```bash
   python -m venv .venv
   ```

2. Activate the virtual environment:
   - On Windows:
     ```bash
     .venv\Scripts\activate
     ```
   - On macOS/Linux:
     ```bash
     source .venv/bin/activate
     ```

3. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

## Setting Up Environment Variables

1. Create a `.env` file in the root directory:

2. Add the following variables to your `.env` file:
   ```
   # Azure OpenAI configuration
   AZURE_OPENAI_API_KEY=your_key_here
   AZURE_OPENAI_ENDPOINT=your_endpoint_here
   OPENAI_API_VERSION=2025-01-01-preview

   # Azure AI Content Safety configuration
   CONTENT_SAFETY_ENDPOINT=your_endpoint_here
   CONTENT_SAFETY_KEY=your_key_here
   ```

3. Replace the placeholder values with your actual Azure AI Content Safety credentials from the Azure portal.

## Run application

```bash
chainlit run chainlit.py -w
```