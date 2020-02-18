all: tp correction
	echo "done"


tp: *.tex
	pdflatex -shell-escape -jobname="elech201_tp1b" main.tex
	pdflatex -shell-escape -jobname="elech201_tp1b" main.tex


correction: *.tex
	pdflatex -shell-escape -jobname=elech201_tp1b_correction "\def\koriG{} \input{main.tex}"
	pdflatex -shell-escape -jobname=elech201_tp1b_correction "\def\koriG{} \input{main.tex}"

clean:
	rm -f elech201_tp1b_correction.pdf rm elech201_tp1b.pdf
	rm -f *.idx *.aux *.log *.nav *.out *.snm *.toc
