NAME = rush-2
CC = gcc
CFLAGS = -Wall -Wextra -Werror
DEPS = ft_rushes.h
OBJ = main.o memory.o rush-02.o stdin_stdout.o

all: $(NAME) $(OBJ)


# we introduce a dependency of .o files
%.o: %.c $(DEPS)
	$(CC) $(CFLAGS) -c -o $@ $<

# creating an executable program
$(NAME): $(OBJ)
	gcc $(CFLAGS) -o $@ $^

# used to clean only object files
clean:
	rm -f $(OBJ)

# used to clean all files
fclean: clean
	rm -f $(NAME)

re: fclean all



