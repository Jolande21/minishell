# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: sgluck <marvin@42.fr>                      +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2023/01/22 18:18:46 by sgluck            #+#    #+#              #
#    Updated: 2023/02/01 16:18:02 by sgluck           ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

NAME = libft.a
CFLAGS = -Wall -Wextra -Werror -I.
CC = cc
SRCS = ft_isalpha.c ft_itoa.c ft_memmove.c ft_putstr_fd.c ft_striteri.c ft_strmapi.c ft_strtrim.c \
             ft_atoi.c ft_isascii.c ft_malloc.c ft_memset.c ft_realloc.c ft_strjoin.c ft_strncmp.c ft_substr.c \
             ft_bzero.c ft_isdigit.c ft_memchr.c ft_putchar_fd.c ft_split.c ft_strlcat.c ft_strndup.c ft_tolower.c \
             ft_calloc.c ft_isprint.c ft_memcmp.c ft_putendl_fd.c ft_strchr.c ft_strlcpy.c ft_strnstr.c ft_toupper.c \
             ft_isalnum.c ft_isspace.c ft_memcpy.c ft_putnbr_fd.c ft_strdup.c ft_strlen.c ft_strrchr.c
OBJS = $(SRCS:.c=.o)
RM = rm -f

all:	$(NAME)

$(NAME): $(OBJS)
	ar rcs $(NAME) $(OBJS)

%.o: %.c
	$(CC) $(CFLAGS) -c $< -o $@

clean:
	$(RM) $(OBJS)

fclean:	clean
	$(RM) $(NAME)

re:	fclean $(NAME)

.PHONY:	all clean fclean re libft
