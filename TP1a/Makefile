all: tp correction
	echo "done"


tp: *.tex
	pdflatex -shell-escape -jobname="elech201_tp1a" main.tex
	pdflatex -shell-escape -jobname="elech201_tp1a" main.tex


correction: *.tex
	pdflatex -shell-escape -jobname=elech201_tp1a_correction "\def\koriG{} \input{main.tex}"
	pdflatex -shell-escape -jobname=elech201_tp1a_correction "\def\koriG{} \input{main.tex}"

clean:
	rm -f elech201_tp1a_correction.pdf rm elech201_tp1a.pdf
	rm -f *.idx *.aux *.log *.nav *.out *.snm *.toc
