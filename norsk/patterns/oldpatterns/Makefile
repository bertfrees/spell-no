# Simple Makefile to translate a TeX readable hyphenation patterns
# file into a Patgen (and human) readable file.

all: nohyph1.txt nohyph2.txt nohyphsimen.txt ukhyph.txt

%.txt: %.tex
	cat $< \
	  | sed -e '1,/^[ 	]*\\patterns/ D' \
                -e 's/\^\^e0/�/g' \
		-e 's/\^\^e1/�/g' \
		-e 's/\^\^e2/�/g' \
		-e 's/\^\^e3/�/g' \
		-e 's/\^\^e4/�/g' \
		-e 's/\^\^e5/�/g' \
		-e 's/\^\^e6/�/g' \
		-e 's/\^\^e7/�/g' \
		-e 's/\^\^e8/�/g' \
		-e 's/\^\^e9/�/g' \
		-e 's/\^\^ea/�/g' \
		-e 's/\^\^eb/�/g' \
		-e 's/\^\^ec/�/g' \
		-e 's/\^\^ed/�/g' \
		-e 's/\^\^ee/�/g' \
		-e 's/\^\^ef/�/g' \
		-e 's/\^\^f0/�/g' \
		-e 's/\^\^f1/�/g' \
		-e 's/\^\^f2/�/g' \
		-e 's/\^\^f3/�/g' \
		-e 's/\^\^f4/�/g' \
		-e 's/\^\^f5/�/g' \
		-e 's/\^\^f6/�/g' \
		-e 's/\^\^f7/�/g' \
		-e 's/\^\^f8/�/g' \
		-e 's/\^\^f9/�/g' \
		-e 's/\^\^fa/�/g' \
		-e 's/\^\^fb/�/g' \
		-e 's/\^\^fc/�/g' \
		-e 's/\^\^fd/�/g' \
		-e 's/\^\^fe/�/g' \
		-e 's/\^\^ff/�/g' \
		-e '/\}/,$$ D' \
	  > $@

clean:
	-rm -f nohyph1.txt nohyph2.txt nohyphsimen.txt ukhyph.txt
