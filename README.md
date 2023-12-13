# tex-elsevier-template

Git repo for the LaTeX elsevier template, together with cover letter and response letter template and auto compiling on github.

* Response letter template is based on [klb2/review-response-template](https://github.com/klb2/review-response-template)
* Cover letter template is based on [NJU cover_Letter Template](https://www.overleaf.com/latex/templates/nju-cover-letter-template-nan-da-tou-gao-xin-mo-ban/tkdpzmwxvksw)

## Usage

* click 'use this template' to create repo based on this one.
* write your paper in `MANUSCRIPT.tex` and modify other related files.
* compile the local file with `latex` or `pdflatex`.
* git push with a tag will trigger github action to compile `AUTHOR_STATEMENT.tex`, `COVER_LETTER.tex`, `MANUSCRIPT.tex` and `RESPONSE_LETTER.tex` to pdf and attach these pdfs to a new release. Example:
```bash
git commit -m "add release with a tag"
git tag -a v1.0.23.12.13 -m "tag info"
git push origin master
git push origin v1.0.23.12.13
```
Note that the read/write permission of workflow shoule be enabled first. Set this in Repository Settings -> Actions -> General -> Workflow Permissions. You should see the generated PDF in the release page.