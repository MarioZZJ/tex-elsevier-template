# tex-elsevier-template

Git repo for the LaTeX elsevier template, together with cover letter and response letter template and auto compiling on github.

* Response letter template is based on [klb2/review-response-template](https://github.com/klb2/review-response-template)
* Cover letter template is based on [NJU cover_Letter Template](https://www.overleaf.com/latex/templates/nju-cover-letter-template-nan-da-tou-gao-xin-mo-ban/tkdpzmwxvksw)

## Usage

* click 'use this template' to create repo based on this one.
* write your paper in `MANUSCRIPT.tex` and modify other related files.
* compile the local file with `latex` or `pdflatex`.
* git push with a tag will trigger github action to compile `AUTHOR_STATEMENT.tex`, `COVER_LETTER.tex`, `MANUSCRIPT.tex` and `RESPONSE_LETTER.tex` to pdf and attach these pdfs to a new release.