Old model (using Logistic Regression): [HuggingFace Spaces link](https://huggingface.co/spaces/sohomghosh/FinRead) <br>
Old model (using lightgbm classifier): [Google Colab link](https://colab.research.google.com/drive/18K_X_sONhA0SHIl96c-KUyhwlOFLtp1z?usp=sharing)

![alt text](https://github.com/sohomghosh/FinRAD_Financial_Readability_Assessment_Dataset/blob/main/old_model_FinRead/FinRead_gradio.png)


The folder [FinRead_ICON2021_Demo](https://github.com/sohomghosh/FinRAD_Financial_Readability_Assessment_Dataset/tree/main/old_model_FinRead/FinRead_ICON2021_Demo) contains the notebook [FinRead_ICON21_Demo_Readability_System.ipynb](https://github.com/sohomghosh/FinRAD_Financial_Readability_Assessment_Dataset/blob/main/old_model_FinRead/FinRead_ICON2021_Demo/FinRead_ICON21_Demo_Readability_System.ipynb) which was presented as a demo at ICON 2021 (http://icon2021.nits.ac.in/coloc_events.html). It is a lightgbm model trained on FinBERT embeddings extracted using sentence transformers.

NOTE: You need to load the artifact [clf_lgbm_finbert.pickle](https://github.com/sohomghosh/FinRAD_Financial_Readability_Assessment_Dataset/blob/main/old_model_FinRead/FinRead_ICON2021_Demo/clf_lgbm_finbert.pickle) while executing the notebook. This is a LightGBM classifier trained over FinBERT sentence embeddings of more than 8000 definitions of financial terms.



**Our new dataset FinRAD and related models are more advanced an enhanced than this one.**


```bibtex 
@proceedings{ghosh-2021-finread,
    title = "FinRead: A Transfer Learning Based Tool to Assess Readability of Definitions of Financial Terms",
    author = "Sohom Ghosh, Shovon Sengupta, Sudip Kumar Naskar, Sunny Kumar Singh",
    booktitle = "Proceedings of the 18th International Conference on Natural Language Processing (ICON) : 
 System Demonstrations",
    month = "dec",
    year = "2021",
    publisher = "NLP Association of India (NLPAI)",
    url = "forthcoming",
    intype = {to appear in},
    pre-print = "https://easychair.org/publications/preprint/1wvS"
}
```
