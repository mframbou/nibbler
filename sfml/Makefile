CC = g++
CPPFLAGS = -Wall -Wextra -Werror -fPIC -O3 -std=c++11 -I../include-sfml
LDFLAGS = -lsfml-graphics -lsfml-window -lsfml-system -lsfml-audio -L../lib-sfml

NAME = libnibbler_sfml.so

SRCS = $(wildcard *.cpp)
OBJS = $(SRCS:.cpp=.o)

$(NAME): $(OBJS)
	$(CC) $(CPPFLAGS) -shared $(OBJS) -o $(NAME) $(LDFLAGS)

clean:
	rm -f $(OBJS)

fclean: clean
	rm -f $(NAME)

re: fclean $(NAME)
