# 定义目标文件 "main"
# 该目标依赖于目标文件 "math.o" 和 "main.o"
# 通过gcc链接生成可执行文件 "main"
main: math.o main.o
	gcc -o main math.o main.o

# 定义目标文件 "math.o"
# 它依赖于源文件 "math.c" 和头文件 "Math.h"
# 通过gcc编译生成目标文件 "math.o"
math.o: math.c Math.h
	cc -c math.c

# 定义目标文件 "main.o"
# 它依赖于源文件 "main.c" 和头文件 "Math.h"
# 通过gcc编译生成目标文件 "main.o"
main.o: main.c Math.h
	cc -c main.c

# 定义伪目标 "clean"
# 用于清理生成的目标文件和可执行文件
clean:
	rm -rf math.o main.o
