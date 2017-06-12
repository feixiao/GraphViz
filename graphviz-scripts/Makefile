
DOT_SRC_FILES = $(wildcard *.dot)
DOT_PDF_FILES = $(patsubst %.dot,%.jpg,${DOT_SRC_FILES})

default : ${DOT_PDF_FILES} 


${DOT_PDF_FILES} : %.jpg : %.dot
	dot -Tjpg -Gdpi=300 $< > $@


.PHONY : default clean

default : ${TEX_PDF_FILES}

clean : 
	rm *.jpg
