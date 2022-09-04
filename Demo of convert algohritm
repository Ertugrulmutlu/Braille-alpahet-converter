#include <iostream>
#include <stdio.h>
#include <bits/stdc++.h>

/*
English:
Coded By Ertu�rul Mutlu
Please do not copy without any permission

T�rk�e:
Ertu�rul Mutlu taraf�ndan kodlanm��t�r.
L�tfen izinsiz kopyalamay�n�z.

Espa�ol:
Codificado por Ertu�rul Mutlu.
Por favor no copie sin permiso
*/
using namespace std;
int getrusage(int who, struct rusage *usage);
void sep_left_right(string word,string r_word){
	if (r_word.c_str() != NULL){
		printf("\nfor to %s : \n",r_word.c_str());	
		for (int i = 0; i < word.length(); i++ ){
			if( word[i] == '9'){
				printf("right: ");
				for (int z =1; z < 3 ;z++){
					if(word[i+z] != '8'){
						printf("\n %c \n",word[i+z]);
					}
				}
			}
			else if (word[i] =='8'){
				printf("left:");
				for(int z=1; z<3;z++){
					if(word[i+z] != '9'){
						printf("\n %c \n" , word[i+z]);
					}
				}
			}
		}
	}
	else{
	 	printf("Done");	
	}
}


void rsc(string s, string a) /* This function scrap speacial char like ":", "_" */
{
    for (int i = 0; i < s.size(); i++) {
        if (s[i] < '1' || s[i] > '9')
        {  
            s.erase(i, 1);
            i--;
        }
    }
    sep_left_right(s,a.c_str());
}

void proc(char word[] ,char list1[][2], char list2[][29]){/*That is the main code of program*/
	int size = strlen(word);
		
	for (int i=0; i< size; i++){
		for (int a=0; a < size; a++){
			if (word[i] == list1[a][0]){/* We compare the letter with list*/
			rsc(list2[a],list1[a]); /*We delete the character and print it to see it on the screen*/
	    	continue;
				}		
		}
	}	
}
int main() {
	char alp[][2] = {"a","b","c"}; /*Alpahet list*/
	char b_alp[][29] = {"8_1:","8_1_2:","8_1:9_1"};/*BraInt  list*/
	
	char word[64];/*definition of the character */
	scanf("%s",word);/*get the character*/
	proc(word,alp,b_alp);/*We run the main program*/
	

}
