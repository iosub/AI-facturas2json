# Facturas2json

This project is a Streamlit application designed to extract information from PDF invoices and convert it into a structured format (JSON).

## Features

- User interface in Spanish
- Multiple PDF file upload
- PDF text extraction using the Marker library
- Structured data extraction using a nuExtract foundation model
- PDF preview and extracted data editing
- Data saving in JSONL format
- Background processing to improve efficiency

## System Requirements

- Python 3.8 or higher
- Additional libraries specified in `requirements.txt`

## Installation

1. Clone this repository:
   ```
   git clone https://github.com/lahoramaker/facturas2json.git
   cd facturas2json
   ```

2. Create a virtual environment (optional but recommended):
   ```
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. Install the dependencies:
   ```
   pip install -r requirements.txt
   ```

## Usage

1. Run the application:
   ```
   streamlit run facturas2json.py
   ```

2. Open your web browser and go to the address shown in the console (usually http://localhost:8501).

3. Use the interface to upload PDF files, review the extracted data, and save the results.

## Invoice analyzer

A new feature has beed added to analyze the extracted invoices. It also allows you convert from JSON to CSV and viceversa. To execute it, execute the following command:


   ```
   streamlit run src/analizar_facturas.py
   ```

If this script is not in your local repo, please update it executing `git pull`.

## Notes

- Make sure your PDFs are readable and in a standard format for best results.
- The application uses AI models for data extraction, so results may vary depending on the quality and format of the PDFs.
- Please note that the Marker weights for the models are licensed cc-by-nc-sa-4.0, but waived by the author that for any organization under $5M USD in gross revenue in the most recent 12-month period AND under $5M in lifetime VC/angel funding raised. If you'd like to know more about the licensing, please visit the [Marker repository](https://github.com/VikParuchuri/marker)

## Additional resources

To learn more about the project, you can check the following videos (in Spanish):
- Aplication overview: https://youtu.be/I7N2DSzUXbc
- Demo plus detailed description of componentes and code: https://youtu.be/Gov8eR5LBHQ

## Contributing

Contributions are welcome. Please open an issue to discuss significant changes before creating a pull request.

## License

[MIT](https://choosealicense.com/licenses/mit/)
