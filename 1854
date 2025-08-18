int maximumPopulation(int** logs, int logsSize, int* logsColSize) {
    int life[101] = {0};
    for (int i=0; i<logsSize; i++){
        int birth = logs[i][0];
        int death = logs[i][1];
        life[birth - 1950]++;
        life[death - 1950]--;
    }

    int maxpop = 0 , current_pop =  0, year = 0;
    for (int i = 0; i<101  ; i++){
        current_pop += life [i];
        if (current_pop >maxpop){
            maxpop = current_pop;
            year = i + 1950;
        }
    }
    return year;
}
