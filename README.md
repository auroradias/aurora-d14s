```c
#include <stdio.h>

void printSkills(const char *category, const char *skills[], int size) {
    printf("%s: ", category);
    for (int i = 0; i < size; i++) {
        printf("%s", skills[i]);
        if (i < size - 1) printf(", ");
    }
    printf("\n");
}

int main() {
    const char *clientSkills[] = {"C", "C++"};
    const char *serverDatabaseSkills[] = {"MySQL"};
    const char *studying[] = {"Logic Programming", "Algorithm Optimization"};

    printSkills("Programming Languages", clientSkills, 2);
    printSkills("Server & Database", serverDatabaseSkills, 1);
    printSkills("Studying", studying, 2);

    return 0;
}
```
