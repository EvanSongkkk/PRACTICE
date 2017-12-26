# oj
#include <stdio.h>

int main(int argc, const char * argv[]) {
    int n,nn,i,time,t;
    int num[1000],new[1000];
    scanf("%d",&n);
    for(nn=0;nn<n;nn++)
        scanf("%d",&num[nn]);
    new[0]=num[0];
    for(time=1;time<n;time++)    //num中抽取
    {
        for(i=0;i<time;i++)       //new中插入
        {
            if(new[i]>num[time])      //在哪里插入
            {
                for(t=time;t>i;t--)     //从i处后移
                    new[t]=new[t-1];
                new[i]=num[time];
             //   printf("%d",new[i]);
                break;
            }
            else
                new[time]=num[time];
        }
    }
    for(nn=0;nn<n;nn++)
        printf("%d ",new[nn]);
    printf("\n");
    return 0;
}
