#include <stdio.h>
#include <string.h>

int main() {
    int i;
    char state[4][20] = {"maharashtra", "kerala", "goa", "assam"};
    char capital[4][20] = {"mumbai", "thiruvananthapuram", "panaji", "dispur"};
    char inputstate[20];

    printf("Enter the state name: ");
    scanf("%s", inputstate);

    for (i = 0; i < 4; i++) {
        if (strcmp(inputstate, state[i]) == 0) {
            printf("Capital of state %s is %s\n", state[i], capital[i]);
        }
    }

    return 0;
}
