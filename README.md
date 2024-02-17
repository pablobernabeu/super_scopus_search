
# rscopus_plus

## A little extension of the `rscopus` package

These functions provide a modest extension of the R package [`rscopus`](https://github.com/muschellij2/rscopus) to administer the search quota and to make specific searches and comparisons. An example of use is [available here](https://github.com/pablobernabeu/L2_L3_EF).

- `scopus_search_plus` runs `rscopus::scopus_search` as many times as necessary based on the number of results and the search quota.

- `scopus_search_DOIs` gets DOIs from `scopus_search_plus`, which can then be imported into a reference manager, such as Zotero, to create a list of references.
  
- `scopus_search_additional_DOIs` searches for additional DOIs.

- `scopus_comparison` compares counts of publications on various topics during a certain period.

- `plot_scopus_comparison` draws a line plot with the output from `scopus_comparison`.

    ![plot_L2_L3_EF](https://raw.githubusercontent.com/pablobernabeu/L2_L3_EF/main/plot_L2_L3_EF.svg)

---

*Note.* Before using any of these functions, the user must read in their Scopus API key confidentially (see [rscopus guidelines](https://cran.r-project.org/web/packages/rscopus/vignettes/api_key.html)). An error appears if the key has not been read in.
