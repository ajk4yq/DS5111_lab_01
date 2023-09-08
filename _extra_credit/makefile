default:
	@cat

pg1065.txt:
	wget https://www.gutenberg.org/cache/epub/1065/pg1065.txt

raven_lines.txt:
	cat pg1065.txt | grep -i 'raven' > raven_lines.txt

number_of_Raven.txt:
	cat pg1065.txt | grep 'Raven' | wc -l > number_of_Raven.txt

number_of_RAVEN.txt:
	cat pg1065.txt | grep 'RAVEN' | wc -l > number_of_RAVEN.txt

number_of_raven.txt:
	cat pg1065.txt | grep 'raven' | wc -l > number_of_raven.txt

.PHONY: all clean
all: pg1065.txt raven_lines.txt number_of_RAVEN.txt number_of_Raven.txt number_of_raven.txt

clean:
	rm pg1065.txt || true
	rm raven_lines.txt || true
	rm number_of_Raven.txt || true
	rm number_of_RAVEN.txt || true
	rm number_of_raven.txt || true
