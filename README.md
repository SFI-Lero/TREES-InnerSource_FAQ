# InnerSource FAQ

## **Aim**

Creating a master document for various InnerSource FAQs that can easily be translated without too much hassle. The master document ensures that all translations are equivalent

## **Progress**

The `InnerSourceFAQ/InnerSourceFAQ.Rmd` file is  the master document. All text requiring translation are enclosed inside the `i18n$t()` R function.

The translation language can be set in the beginning of the text: `i18n$set_translation_language("<language>")`. The translation file should be in the `./data/translation_<language>.csv` file relative to the `.Rmd` file.

Use the `translation_extract.py` script to extract the text that would require translation.

The output HTML can be viewed as a plain text HTML, however, if the interactivity is desired, the file must be hosted in a *Shiny server*. See <https://rstudio.github.io/learnr/publishing.html> for details of hosting.

## **Quiz**

An interactive quiz is added for assessing the participants' knowledge about InnerSource. The quiz is only available if the file is hosted in a Shiny server. Quiz progress is automatically saved and it is also possible to start over.
