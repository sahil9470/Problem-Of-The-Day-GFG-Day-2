# Problem-Of-The-Day-GFG-Day-2
Array Operations || 12 May 2023 || GFG Solution 

int arrayOperations(int n, vector<int> &a) {
        int count=0, f=1;
        for(int i=0; i<n; i++){
            if(a[i]>0){
                count+=f;
                f=0;
            }
            if(a[i]==0){
                f=1;
            }
        }
        return count;
    }
