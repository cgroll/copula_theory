PICS_FILE_NAMES_1 := $(wildcard rvine_conversion_vertical*)
PICS_FILE_NAMES_2 := $(wildcard rvine_conversion_horizontal*)

SVG_FILES := $(PICS_FILE_NAMES_1) $(PICS_FILE_NAMES_2)
PNG_FILES := $(patsubst %.svg,pngs/%.png,$(SVG_FILES))

png: $(PNG_FILES)

# conversion rule
pngs/%.png: %.svg
	inkscape --export-png=$@ --export-background=white $<	
