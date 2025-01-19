{

    int vetor_repetidos(int vetor_da_silva[], int tam, int num){
        int total = 0;
        
        for (int i=0; i<tam; i++){
            if (vetor_da_silva[i] == num){
                total++;
            }
        }
        
        return total;
    }
}
{

    int sort_crescente(int vetor_da_silva[], int tam){
        int p;
        
        for (int i=0; i<tam; i++){
            for (int j=0; j<tam - 1; j++){
                if (vetor_da_silva[j+1] < vetor_da_silva[j]){
                    p = vetor_da_silva[j];
                    vetor_da_silva[j] = vetor_da_silva[j+1];
                    vetor_da_silva[j+1] = p;
                } 
            }
        }
        
        return *vetor_da_silva;
    }
}
{

    int sort_decrescente(int vetor_da_silva[], int tam){
        int p;
        
        for (int i=0; i<tam; i++){
            for (int j=0; j<tam - 1; j++){
                if (vetor_da_silva[j+1] > vetor_da_silva[j]){
                    p = vetor_da_silva[j];
                    vetor_da_silva[j] = vetor_da_silva[j+1];
                    vetor_da_silva[j+1] = p;
                } 
            }
        }
        
        return *vetor_da_silva;
    }
}
{

    int vetor_print(int vetor_da_silva[], int tam){
        for (int i=0; i<tam; i++){
            printf("%d ", vetor_da_silva[i]);
        }
        printf("\n");
    }
}
{

    int mdc(int a, int b){
        int i = 1;
        int maiorzin = 1;
        
        while (a / i >= 1 && b / i >= 1){
            if (a % i == 0 && b % i == 0){
                maiorzin = i;
            }
            
            i++;
        }
        
        return maiorzin;
    }
}
{

    int eh_primo(int num){
        int i = 2;
        int ehs_primo = 1;
        
        while (num / i >= 2){
            if (num % i == 0){
                return 0;
                ehs_primo = 0;
            }
            
            i++;
        }
        
        if (ehs_primo == 1){
            return 1;
        }
    }
}
