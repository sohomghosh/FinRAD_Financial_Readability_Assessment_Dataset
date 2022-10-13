# FinRAD: Financial Readability Assessment Dataset - 13,000+ Definitions of Financial Terms for Measuring Readability

This repository contains 2 samples ([sample-1](https://github.com/sohomghosh/FinRAD_Financial_Readability_Assessment_Dataset/blob/main/data_sample_500.csv), [sample-2](https://github.com/sohomghosh/FinRAD_Financial_Readability_Assessment_Dataset/blob/main/data_sample_1500.csv)) from the dataset mentioned in the paper: **FinRAD: Financial Readability Assessment Dataset - 13,000+ Definitions of Financial Terms for Measuring Readability** (accepted at The Financial Narrative Processing Workshop colocated with LREC-2022, Marseille, France).

In addition to this, [data collection & cleaning scripts](https://github.com/sohomghosh/FinRAD_Financial_Readability_Assessment_Dataset/tree/main/data_collection_cleaning_EDA_scripts), [embedding extraction & model development script](https://github.com/sohomghosh/FinRAD_Financial_Readability_Assessment_Dataset/blob/main/FinRAD_Sentence_FinBERTembedding_Extraction_Modeling_13K.ipynb), and a [starter example](https://github.com/sohomghosh/FinRAD_Financial_Readability_Assessment_Dataset/blob/main/FinRAD_starting_toy_example_on_data_sample_500.ipynb) are also present. You can dowloand the model along with the weights from [Hugging Face](https://huggingface.co/sohomghosh/finrad_model).

The embeddings & labels of the full dataset are available in the [embeddings_and_labels](https://github.com/sohomghosh/FinRAD_Financial_Readability_Assessment_Dataset/tree/main/embeddings_and_labels) directory. Several model artifacts developed by training classiers like Logistic Regression, GBM, Random Forest on the entire dataset have been made available in the [models](https://github.com/sohomghosh/FinRAD_Financial_Readability_Assessment_Dataset/tree/main/models)  directory.

To access the raw version of the full dataset, please send a request by filling [this form](https://forms.gle/hze6qSPc84kuY3McA). You can also re-create the raw datasets using the [data collection & cleaning scripts](https://github.com/sohomghosh/FinRAD_Financial_Readability_Assessment_Dataset/tree/main/data_collection_cleaning_EDA_scripts/).

![alt text](https://github.com/sohomghosh/FinRAD_Financial_Readability_Assessment_Dataset/blob/main/process_flow.png)

## Metadata of FinRAD
**Primary Columns:** <br>
"terms": _This is the financial term_ <br>
"definitions": _This is the definition corresponding to the financial term_ <br>
"source": _This represents the source from which the term and the definition has been obtained._ <br>
"assigned_readability": _This is the manually assigned readability. 0 means not readable, 1 means readable._<br>

**Other Columns:** <br>
"flesch_reading_ease",	"flesch_kincaid_grade",	"smog_index",	"coleman_liau_index",	"automated_readability_index",	"dale_chall_readability_score",	"linsear_write_formula",	"gunning_fog"<br>
_These are readability scores extracted using the [textstat](https://pypi.org/project/textstat/) library_

**Metadata of source**<br>
|Tag                |Description                                                                                  |Assigned Readability|
|-------------------|---------------------------------------------------------------------------------------------|--------------------|
|prin               |_Principles of Corporate Finance_ by Richard A. Brealey, Stewart C. Myers, Franklin Allen  |0                   |
|zvi                |_Investments_ by Zvi Bodie Alex Kane Alan J. Marcus                                        |0                   |
|sam                |_Economics Textbook_ by Paul Samuelson and William Nordhaus                                |1                   |
|opod               |_Options, Futures, and Other Derivatives, Global Edition_ by John C. Hull                  |0                   |
|fmi                |_Financial Markets and Institutions_ by Frederic S. Mishkin Stanley Eakins                 |0                   |
|ncert_keec111      |_NCERT Indian Economic Development Economics_ Class 11                                     |1                   |
|ncert_kest         |_NCERT Statistics for Economics_ Class 12                                                  |1                   |
|ncert              |_NCERT Introduction to MacroEconomics_ Class 12                                            |1                   |
|ncert_class12_econ |_NCERT Introduction to MicroEconomics_ Class 12                                            |1                   |
|investopedia       |_Investopedia_ Data Dictionary                                                             |1                   |
|economist          |_The Economist_ terms dictionary                                                           |1                   |
|6_8_louis          |_Glossary of Economics and Personal Finance Terms_ from Federal Reserve Bank of St. Louis  |1                   |
|9_12_louis         |_Glossary of Economics and Personal Finance Terms_ from Federal Reserve Bank of St. Louis  |1                   |
|pre_louis          |_Glossary of Economics and Personal Finance Terms_ from Federal Reserve Bank of St. Louis  |1                   |
|palgrave           |_The Palgrave Macmillan Dictionary of Finance, Investment and Banking_ by Erik Banks       |0                   |       

## Citing & Authors
If you find this repository helpful, feel free to cite our forthcoming publication [FinRAD: Financial Readability Assessment Dataset - 13,000+ Definitions of Financial Terms for Measuring Readability](to be updated):
```bibtex 
@InProceedings{ghosh-EtAl:2022:FNP,
  author    = {Ghosh, Sohom  and  Sengupta, Shovon  and  Naskar, Sudip Kumar and  Singh, Sunny Kumar},
  title     = {FinRAD: Financial Readability Assessment Dataset - 13,000+ Definitions of Financial Terms for Measuring Readability},
  booktitle      = {Proceedings of the The 4th Financial Narrative Processing Workshop @LREC2022},
  month          = {June},
  year           = {2022},
  address        = {Marseille, France},
  publisher      = {European Language Resources Association},
  pages     = {1--9},
  url       = {http://www.lrec-conf.org/proceedings/lrec2022/workshops/FNP/pdf/2022.fnp-1.1.pdf}
}
```
and our demo/tool presented at [ICON 2021](http://icon2021.nits.ac.in/coloc_events.html). The artifacts of this demo are available in the [old_model_FinRead](https://github.com/sohomghosh/FinRAD_Financial_Readability_Assessment_Dataset/tree/main/old_model_FinRead) directory. <br>
New model trained on 13K+ instances (using Logistic Regression): [HuggingFace Spaces link](https://huggingface.co/spaces/sohomghosh/FinRead) <br>
Old model trained on 8K+ instances (using lightgbm classifier): [Google Colab link](https://colab.research.google.com/drive/18K_X_sONhA0SHIl96c-KUyhwlOFLtp1z?usp=sharing)

```bibtex 
@inproceedings{ghosh-etal-2021-finread,
    title = "{F}in{R}ead: A Transfer Learning Based Tool to Assess Readability of Definitions of Financial Terms",
    author = "Ghosh, Sohom  and
      Sengupta, Shovon  and
      Naskar, Sudip  and
      Singh, Sunny Kumar",
    booktitle = "Proceedings of the 18th International Conference on Natural Language Processing (ICON)",
    month = dec,
    year = "2021",
    address = "National Institute of Technology Silchar, Silchar, India",
    publisher = "NLP Association of India (NLPAI)",
    url = "https://aclanthology.org/2021.icon-main.81",
    pages = "658--659"
    }
```
![alt text](https://github.com/sohomghosh/FinRAD_Financial_Readability_Assessment_Dataset/blob/main/old_model_FinRead/FinRead_gradio.png)



Contact: sohom1ghosh@gmail.com



For any part of this work for which the license is applicable, this work is licensed under the Creative Commons Attribution-NonCommercial-ShareAlike 4.0 Internationallicense. See [LICENSE.CC-BY-NC-SA-4.0](https://github.com/sohomghosh/FinRAD_Financial_Readability_Assessment_Dataset/blob/main/LICENSE).

