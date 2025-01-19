int vetor_repetidos(int vetor_da_silva[], int tam, int num){
    int total = 0;
    
    for (int i=0; i<tam; i++){
        if (vetor_da_silva[i] == num){
            total++;
        }
    }
    
    return total;
}

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

int vetor_print(int vetor_da_silva[], int tam){
    for (int i=0; i<tam; i++){
        printf("%d ", vetor_da_silva[i]);
    }
    printf("\n");
}
