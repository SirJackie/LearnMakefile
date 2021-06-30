# 第一层:
# Target:Dependence
# 	Command

# .PHONT:
# PhonyTarget:
# 	Command

# 第二层:
# a = b
# a += b
# a := b
# $(a)

# 第三层:
# %.o %.c
# *.o *.c

# 第四层:
# $^   All the dependences
# $@   All the targets

# 第五层:
# 使用函数

Target = test
Objects = main.o circle.o
EditorRubbish = .vscode
CC := gcc
RMRF := rm -rf

$(Target):$(Objects)
	$(CC) $^ -o $@

%.o:%.c
	gcc -c $^ -o $@

.PHONY:
run:
	make
	chmod 777 $(Target)
	./$(Target)

clear:
	$(RMRF) $(EditorRubbish) $(Objects) $(Target)
