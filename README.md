
# Porter6: Secondary Structure Prediction

This pipeline automates the process of predicting secondary structures using multiple tools, providing both 3-class and 8-class secondary structure predictions.

## Requirements

Ensure you have the following dependencies installed before running the pipeline:

- **Python 3.x**
- **Biopython**: Install using `pip install biopython`
- **Torch**: Install using `pip install torch`

You can install all dependencies by running:

```bash
pip install -r requirements.txt
How to Use
1. Download the Pipeline
You can download the pipeline by cloning the repository or downloading the ZIP file directly.

Option 1: Clone the Repository
If you have Git installed, you can clone the repository:

bash
Copy code
git clone https://github.com/WafaAlanazi/Porter6.git
cd Porter6
Option 2: Download the ZIP
Alternatively, you can download the porter6.zip file directly from the GitHub repository and extract it:

bash
Copy code
wget https://github.com/WafaAlanazi/Porter6/raw/main/porter6.zip
unzip porter6.zip
cd porter6
2. Place Your FASTA File
Place your input FASTA file in the data/dataset/ folder. The FASTA file must be named set3.fasta to be processed by the pipeline.

3. Make the Script Executable
Before running the pipeline, ensure that the porter6.sh script is executable. You only need to do this once:

bash
Copy code
chmod +x porter6.sh
4. Run the Pipeline
Once your FASTA file is in place, you can run the entire pipeline by executing the following command:

bash
Copy code
./porter6.sh
5. View the Results
The pipeline will generate secondary structure predictions for both the 3-class and 8-class categories. The results will be saved in the following CSV and JSON files:

predictor3/output_predictions.csv: Contains the 3-class predictions (Q3).
predictor8/output_predictions.csv: Contains the 8-class predictions (Q8).
After the pipeline runs, these two files will be automatically concatenated into a single output file with columns for id, q3, and q8.





