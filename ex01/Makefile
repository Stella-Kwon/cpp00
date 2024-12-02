# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: skwon2 <skwon2@student.hive.fi>            +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2024/11/26 16:48:37 by skwon2            #+#    #+#              #
#    Updated: 2024/12/02 22:37:59 by skwon2           ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

NAME = Phonebook_App

COMPILER = c++

SRC = 	main.cpp \
		main_utils.cpp\
		cmd_add_exit.cpp\
		cmd_search.cpp\
		ContactGet.cpp\
		ContactSet.cpp\
		ContactUtils.cpp\
		PhoneBook.cpp

FLAGS = -Wall -Wextra -Werror -std=c++20

INC = -I.

OBJ = $(SRC:.cpp=.o)

all: $(NAME)

$(NAME) : $(OBJ)
	@$(COMPILER) $(FLAGS) $(INC) -o $(NAME) $(OBJ)
	@echo "\n$(Red)......WAIT$(Ending)\n"
	@echo "$(Green)-----------$(Ending)"
	@echo "$(Green)-------------- $(Ending)"
	@echo "$(Green)------------------- $(Ending)"
	@echo "$(Green)---------------------- $(Ending)"
	@echo "$(Green)--------------------------$(Ending)"
	@echo "$(Green)------------------------------"
	@echo "\n$(Yellow)=> $(NAME) HAS BEEN CREATED$(Ending)\n"

%.o : %.cpp
	@$(COMPILER) $(FLAGS) -c $< -o $@

clean :
	@rm -f $(OBJ)

fclean : clean
	@rm -f $(NAME)

re : fclean all

.PHONY: all clean fclean re

Red = \033[0;31m
Green = \033[0;32m
Yellow = \033[0;33m
Blue = \033[0;34m
Magenta = \033[0;35m
Cyan = \033[0;36m
White = \033[0;37m
Ending = \033[0m