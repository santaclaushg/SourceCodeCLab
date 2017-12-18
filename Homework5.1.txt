#include <stdio.h>
#include <stdlib.h>

int main()
{
    char ch1, ch2, ch3, chmin;
    printf("Enter three characters: ");
    scanf("%c%c%c", &ch1, &ch2, &ch3);
    chmin = ch1;
    if(ch2 < chmin){
        if(ch3 < chmin){
            chmin = ch3;
        }
        else {
            chmin = ch2;
        }
    }
    if(ch3 < chmin){
        chmin = ch3;
    }
    printf("The first alphabetically character is: %c\n", chmin);

    return 0;
}
