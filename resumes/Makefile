RESUME_TEX = Ruming_Liu_Resume.tex
RESUME_PDF = Ruming_Liu_Resume.pdf
CV_TEX = Ruming_Liu_Academic_CV.tex
CV_PDF = Ruming_Liu_Academic_CV.pdf

.PHONY: all clean distclean

all: $(RESUME_PDF) $(CV_PDF)

$(RESUME_PDF): $(RESUME_TEX)
	latexmk -pdf -interaction=nonstopmode -halt-on-error $(RESUME_TEX)

$(CV_PDF): $(CV_TEX)
	latexmk -pdf -interaction=nonstopmode -halt-on-error $(CV_TEX)

clean:
	latexmk -c $(RESUME_TEX)
	latexmk -c $(CV_TEX)

distclean:
	latexmk -C $(RESUME_TEX)
	latexmk -C $(CV_TEX)
