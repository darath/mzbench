
NAME = lua
SOURCES := $(NAME)_worker.lua

$(NAME).tgz: $(SOURCES)
	rm -rf $(NAME)
	mkdir $(NAME)
	cp $(SOURCES) $(NAME)
	tar czf $@ $(NAME)

.PHONY: generate_tgz
generate_tgz: $(NAME).tgz

.PHONY: clean
clean:
	-@rm -f *.tgz
	-@rm -rf data.* log.*
	-@rm -rf $(NAME)