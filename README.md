# FinRAD: Financial Readability Assessment Dataset - 13,000+ Definitions of Financial Terms for Measuring Readability

This repository contains 2 samples ([sample-1](https://github.com/sohomghosh/FinRAD_Financial_Readability_Assessment_Dataset/blob/main/data_sample_500.csv), [sample-2](https://github.com/sohomghosh/FinRAD_Financial_Readability_Assessment_Dataset/blob/main/data_sample_1500.csv)) from the dataset mentioned in the paper: **FinRAD: Financial Readability Assessment Dataset - 13,000+ Definitions of Financial Terms for Measuring Readability** (under review).
In addition to this, data extraction & cleaning scripts, embeddings & labels of the full dataset and few starter examples are also present. To access the full dataset, please send a request by filling this [form](https://forms.gle/hze6qSPc84kuY3McA). We shall share the full dataset after this paper gets accepted.

## Metadata
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
|prin               |Principles of Corporate Finance by Richard A. Brealey, Stewart C. Myers, Franklin Allen  |0                   |
|zvi                |Investments by Zvi Bodie Alex Kane Alan J. Marcus                                        |0                   |
|sam                |Economics Textbook by Paul Samuelson and William Nordhaus                                |1                   |
|opod               |Options, Futures, and Other Derivatives, Global Edition by John C. Hull                  |0                   |
|fmi                |Financial Markets and Institutions by Frederic S. Mishkin Stanley Eakins                 |0                   |
|ncert_keec111      |NCERT Indian Economic Development Economics Class 11                                     |1                   |
|ncert_kest         |NCERT Statistics for Economics Class 12                                                  |1                   |
|ncert              |NCERT Introduction to MacroEconomics Class 12                                            |1                   |
|ncert_class12_econ |NCERT Introduction to MicroEconomics Class 12                                            |1                   |
|investopedia       |Investopedia Data Dictionary                                                             |1                   |
|economist          |The Economist terms dictionary                                                           |1                   |
|6_8_louis          |Glossary of Economics and Personal Finance Terms from Federal Reserve Bank of St. Louis  |1                   |
|9_12_louis         |Glossary of Economics and Personal Finance Terms from Federal Reserve Bank of St. Louis  |1                   |
|pre_louis          |Glossary of Economics and Personal Finance Terms from Federal Reserve Bank of St. Louis  |1                   |
|palgrave           |The Palgrave Macmillan Dictionary of Finance, Investment and Banking by Erik Banks       |0                   |       

## Citing & Authors
If you find this repository helpful, feel free to cite our forthcoming publication [FinRAD: Financial Readability Assessment Dataset - 13,000+ Definitions of Financial Terms for Measuring Readability](to be updated):
```bibtex 
@misc{ghosh-2022-finrad,
    title = "FinRAD: Financial Readability Assessment Dataset - 13,000+ Definitions of Financial Terms for Measuring Readability",
    author = "Sohom Ghosh, Shovon Sengupta, Sudip Kumar Naskar, Sunny Kumar Singh",
    booktitle = "",
    month = "",
    year = "2022",
    publisher = "",
    url = "forthcoming",
    intype = {to appear in},
}
```
and our demo/tool presented at [ICON 2021](http://icon2021.nits.ac.in/coloc_events.html):
```bibtex 
@proceedings{ghosh-2021-finread,
    title = "FinRead: A Transfer Learning Based Tool to Assess Readability of Definitions of Financial Terms",
    author = "Sohom Ghosh, Shovon Sengupta, Sudip Kumar Naskar, Sunny Kumar Singh",
    booktitle = "",
    month = "dec",
    year = "2021",
    publisher = "NLP Association of India (NLPAI)",
    url = "forthcoming",
    intype = {to appear in},
    pre-print = "https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3979016"
}
```




Contact: sohom1ghosh@gmail.com



For any part of this work for which the license is applicable, this work is licensed under the Attribution-NonCommercial-NoDerivatives 4.0 International license. See [LICENSE.CC-BY-NC-ND-4.0](https://github.com/sohomghosh/FinRAD_Financial_Readability_Assessment_Dataset/blob/main/LICENSE).

