# DeepNet
*DeepNet*: *Deep* learning model for predicting HLA-epitope interaction based on *Net* work analysis by harnessing binding and immunogenicity information

In DeepNet model, both binding intensity of HLA-peptide pairs and potential immunogenicity of epitopes which are capable of eliciting CD8+ T cell responses were considered. In addition, to improve model accuracy, network centrality metrics were extracted through network construction which proved to possess sufficient prediction power in comparison. Extensive tests on independent and benchmark datasets demonstrate that DeepNet can significantly outperform other well-known binding prediction tools. 

### Dependencies
DeepNet requires the following Python 3.0 modules:
- numpy 1.16.4
- pandas 0.24.2
- keras 2.2.4
- scipy 1.3.0

###1. Description of input
The input data should meet the following format:

Columns  | Description
------------- | -------------
mhc | mhc class I molecules (e.g. HLA-A01:01)
sequence  | 9-mer peptides (e.g. RTFNEDLFR)

###2. Implementation
You can implement the code as follows:
   ```sh
    python predict.py [inputfile]
   ```
For example:
   ```sh
    python predict.py data/sample.csv
   ```
  
  ###Description of output
  The output 
