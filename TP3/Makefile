all: tp correction
	echo "done"


tp: *.tex
	pdflatex -shell-escape -jobname="elech201_tp3" main.tex
	pdflatex -shell-escape -jobname="elech201_tp3" main.tex


correction: *.tex
	pdflatex -shell-escape -jobname=elech201_tp3_correction "\def\koriG{} \input{main.tex}"
	pdflatex -shell-escape -jobname=elech201_tp3_correction "\def\koriG{} \input{main.tex}"

clean:
	rm -f elech201_tp3_correction.pdf rm elech201_tp3.pdf
	rm -f *.idx *.aux *.log *.nav *.out *.snm *.toc
