# FinRAD: Financial Readability Assessment Dataset - 16,000+ Definitions of Financial Terms for Measuring Readability

This repository contains a sample of the data mentioned in the paper: FinRAD: Financial Readability Assessment Dataset - 16,000+ Definitions of Financial Terms for Measuring Readability (under review). The full data will be released after the acceptance of the paper.

## Metadata
**Primary Columns:** <br>
"terms": _This is the financial term_ <br>
"definitions": _This is the definition corresponding to the financial term_ <br>
"source": _This represents the source from which the term and the definition has been obtained._ <br>
"assigned_readibility": _This is the manually assigned readability_<br>

**Other Columns:** <br>
"flesch_reading_ease",	"flesch_kincaid_grade",	"smog_index",	"coleman_liau_index",	"automated_readability_index",	"dale_chall_readability_score",	"difficult_words",	"linsear_write_formula",	"gunning_fog",	"text_standard",	"fernandez_huerta",	"szigriszt_pazos",	"gutierrez_polini",	"crawford",	"gulpease_index",	"osman" <br>
_These are readability scores extracted using the [textstat](https://pypi.org/project/textstat/) library_

**Metadata of source**<br>
'prin': Principles of Corporate Finance by Richard A. Brealey, Stewart C. Myers, Franklin Allen <br>
'zvi': Investments by Zvi Bodie Alex Kane Alan J. Marcus <br>
'sam': Economics Textbook by Paul Samuelson and William Nordhaus <br>
'opod': Options, Futures, and Other Derivatives, Global Edition by John C. Hull <br>
'fmi': Financial Markets and Institutions by Frederic S. Mishkin Stanley Eakins <br>
'ncert_keec111': <br>
'ncert_kest': <br>
'ncert': keec<br>
'ncert_class12_econ': NCERT Class 12 Economics<br> 
'investopedia': Investopedia Data Dictionary <br>
'economist': The Economist terms dictionary <br>
'6_8_louis': Glossary of Economics and Personal Finance Terms from Federal Reserve Bank of St. Louis <br>
'9_12_louis': Glossary of Economics and Personal Finance Terms from Federal Reserve Bank of St. Louis  <br>
'college_louis': Glossary of Economics and Personal Finance Terms from Federal Reserve Bank of St. Louis  <br>
'non_educators_louis': Glossary of Economics and Personal Finance Terms from Federal Reserve Bank of St. Louis  <br>
'pre_louis': Glossary of Economics and Personal Finance Terms from Federal Reserve Bank of St. Louis  <br>
'palgrave': The Palgrave Macmillan Dictionary of Finance, Investment and Banking by Erik Banks <br>
       
## Citing & Authors
If you find this repository helpful, feel free to cite our forthcoming publication [FinRAD: Financial Readability Assessment Dataset - 16,000+ Definitions of Financial Terms for Measuring Readability](to be updated):
```bibtex 
@misc{ghosh-2022-finrad,
    title = "FinRAD: Financial Readability Assessment Dataset - 16,000+ Definitions of Financial Terms for Measuring Readability",
    author = "Sohom Ghosh, Shovon Sengupta, Sudip Kumar Naskar, Sunny Kumar Singh",
    booktitle = "",
    month = "",
    year = "2022",
    publisher = "",
    url = "forthcoming",
    intype = {to appear in},
}
```


Contact: sohom1ghosh@gmail.com



For any part of this work for which the license is applicable, this work is licensed under the Attribution-NonCommercial-NoDerivatives 4.0 International license. See [LICENSE.CC-BY-NC-ND-4.0](https://github.com/sohomghosh/FinRAD_Financial_Readability_Assessment_Dataset/blob/main/LICENSE).

