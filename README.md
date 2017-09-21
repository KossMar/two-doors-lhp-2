# two-doors-lhp-2
Lighthouse Prep Assignment 2

    
#include <stdio.h>
#include <stdlib.h>

void runGame(char play1, char choice1){
    printf("\nYou are a prisoner in a room with 2 doors and 2 guards.\n");
    printf("One of the doors will guide you to freedom and behind the other is a hangman --you don't know which is which.\n");
    printf("One of the guards always tells the truth and the other always lies. You don't know which one is the truth-teller or the liar either.\n");
    printf("You have to choose and open one of these doors, but you can only ask a single question to one of the guards.\n");
    printf("What do you ask so you can pick the door to freedom?\n\n");
    printf("a.Ask the truth-guard to point to the door of doom.\n");
    printf("b.Ask the liar-guard to point to the door of doom.\n");
    printf("c.Doesn't matter which one you pick.\n");
    scanf("%s", &choice1);
    
    char answer = printf("No matter which one you choose the guards both tell you which door leads to death, and therefore you can pick       the other door.\n");
    
    switch (choice1) {
        case 1:
            printf("%c", answer);
            break;
        case 2:
            printf("%c", answer);
            break;
        case 3:
            printf("%c", answer);
            break;
        default:
            break;
    }
    printf("Play again? (y/n) \n");
    scanf("%s", &play1);
    
    if (play1 == 'y'){
        runGame(play1, choice1);
    }
}

    int main(int argc, const char * argv[]) {
        
        char play;
        char choice = '\0';
        
    
        
        printf("Welcome to Two doors.\n");
        printf("Would you like to play? (y/n): ");
        scanf("%s", &play);
        
        if (play == 'y') {
            runGame(play, choice);
                   }
        else {
         exit(0);
        }
    
        
        return 1;
    }
