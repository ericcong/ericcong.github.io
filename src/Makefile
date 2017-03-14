SRC=$(wildcard *.md)

all: $(SRC)
	@pandoc -f markdown -t html -H ../assets/header.html \
		-B ../assets/before.html \
		-A ../assets/after.html \
		"$?" -o "../$(strip $(basename $(notdir $?) .md)).html"

clean:
	@rm -r ../*.html