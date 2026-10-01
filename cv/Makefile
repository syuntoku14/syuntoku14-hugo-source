# Build resume.pdf with LuaLaTeX and copy it to the website's static folder.
BUILD := build
TARGET := ../static/uploads/resume.pdf

.PHONY: all clean

all: $(TARGET)

$(TARGET): resume.tex
	mkdir -p $(BUILD)
	lualatex -interaction=nonstopmode -halt-on-error -output-directory=$(BUILD) resume.tex
	lualatex -interaction=nonstopmode -halt-on-error -output-directory=$(BUILD) resume.tex
	cp $(BUILD)/resume.pdf $(TARGET)

clean:
	rm -rf $(BUILD)
