# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: gcampbel <marvin@42.fr>                    +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2023/12/24 18:27:04 by gcampbel          #+#    #+#              #
#    Updated: 2023/12/24 18:46:58 by gcampbel         ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

NAME		= libft.a

CC		= cc

FLAGS		= -Wall -Wextra -Werror

SRCS		= ft_atoi.c \
		  ft_bzero.c \
		  ft_calloc.c \
		  ft_isalnum.c \
		  ft_isalpha.c \
		  ft_isascii.c \
		  ft_isdigit.c \
		  ft_isprint.c \
		  ft_itoa.c \
		  ft_memchr.c \
		  ft_memcmp.c \
		  ft_memcpy.c \
		  ft_memmove.c \
		  ft_memset.c \
		  ft_putchar_fd.c \
		  ft_putendl_fd.c \
		  ft_putnbr_fd.c \
		  ft_putstr_fd.c \
		  ft_split.c \
		  ft_strchr.c \
		  ft_strdup.c \
		  ft_striteri.c \
		  ft_strjoin.c \
		  ft_strlcat.c \
		  ft_strlcpy.c \
		  ft_strlen.c \
		  ft_strmapi.c \
		  ft_strncmp.c \
		  ft_strnstr.c \
		  ft_strrchr.c \
		  ft_strtrim.c \
		  ft_substr.c \
		  ft_tolower.c \
		  ft_toupper.c

BONSRCS		= ft_lstadd_back.c \
		  ft_lstadd_front.c \
		  ft_lstclear.c \
		  ft_lstdelone.c \
		  ft_lstiter.c \
		  ft_lstlast.c \
		  ft_lstmap.c \
		  ft_lstnew.c \
		  ft_lstsize.c

OBJS		= $(SRCS:.c=.o)

BONOBJS		= $(BONSRCS:.c=.o)

all:		$(NAME)

$(NAME):	$(OBJS)
			@ar rcs $(NAME) $(OBJS)

%.o: %.c 
		$(CC) $(FLAGS) -c $< -o $@

bonus:		$(OBJS) $(BONOBJS)
			@ar rcs $(NAME) $(OBJS) $(BONOBJS)

clean:
			@rm -f $(OBJS) $(BONOBJS)

fclean:		clean
			@rm -f $(NAME)

re:		fclean all

.PHONY:		all bonus clean fclean re
