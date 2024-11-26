# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: skwon2 <skwon2@student.hive.fi>            +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2024/11/26 14:03:05 by skwon2            #+#    #+#              #
#    Updated: 2024/11/26 15:01:17 by skwon2           ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

NAME = megaphone

COMPILER = c++

SRC = megaphone.cpp

FLAGS = -Wall -Wextra -Werror -std=c++98

OBJ = $(SRC:.cpp=.o)

all: $(NAME)

$(NAME) : $(OBJ)
	@$(COMPILER) $(FLAGS) -o $(NAME) $(OBJ)
	@echo "\n$(Red)......WAIT$(Ending)\n"
	@echo "$(Green)-----------$(Ending)"
	@echo "$(Green)-------------- $(Ending)"
	@echo "$(Green)------------------- $(Ending)"
	@echo "$(Green)---------------------- $(Ending)"
	@echo "$(Green)--------------------------$(Ending)"
	@echo "$(Green)------------------------------"
	@echo "📣 📣 📣 📣 📣 📣 📣 📣 📣 📣 📣"
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