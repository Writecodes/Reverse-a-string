# Reverse-a-string
public class SearchingTech {
    public static void main(String[] args) {
     String[] names={"Prashant","Stuti","Aman","Archit","Rinky"};
        int i,j;
        String temp;
        for (i=0;i<names.length;i++)
        {
            for (j=0;j< names.length-1-i;j++)
            {
                if(names[j].compareTo(names[j+1])>0)
                {
                    temp=names[j+1];
                    names[j+1]=names[j];
                    names[j]=temp;
                }
            }
        }
        System.out.print("Sorted string list : ");
        for (i=0;i<names.length;i++)
            System.out.print(names[i]+" ");
    }
}
