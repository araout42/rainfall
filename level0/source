#include <stdio.h>
#include <strings.h>
#include <stdlib.h>
#include <unistd.h>
#include <sys/types.h>

int main(int ac, char **av)
{
	if (atoi(av[1]) == 423)
	{
		char *a[2];
		a[0] = strdup("/bin/sh");
		int g = getgid();
		int u = getuid();
		setresgid(g, g, g);
		setresuid(u, u, u);
		execv("/bin/sh", a);
	}
	else
		fwrite("No !\n", 1, 5, stderr);
	return (0);
}
