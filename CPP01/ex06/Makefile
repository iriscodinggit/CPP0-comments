NAME    = harlFilter
CFLAG   = c++ -Wall -Werror -Wextra -std=c++98
RM      = rm -rf
SOURCES =  main.cpp Harl.cpp
OBJECTS = $(SOURCES:%.cpp=%.o)
PINK = \033[38;5;218m

%.o: %.cpp
	@$(CFLAG) -c $< -o $@

$(NAME): $(OBJECTS)
	@$(CFLAG) $(OBJECTS) -o $(NAME)
	@echo "$(PINK)👨‍💻 harlFilter compiled! Usage -> ./harlFilter DEBUG/INFO/WARNING/ERROR"

clean : 
	@$(RM) $(OBJECTS)
	@echo "$(PINK) Objects removed 🧹"

fclean : clean
	@$(RM) $(NAME)
	@echo "$(PINK) Project cleaned 🧹"

all : $(NAME)

re: fclean all

.PHONY: clean all re fclean