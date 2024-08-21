### 1) Sum Triangle 

```
class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Try programiz.pro");
        int nums[]={1,2,3,4,5};
        sumTraingle(nums);
        for(int i=0;i<nums.length;i++){
            System.out.print(nums[i]+" ");
        }
    }
    static void sumTraingle(int nums[]){
        if(nums.length==1){
           // System.out.println(nums[0]);
            return;
        }
        int arr[] = new int[nums.length-1];
        for(int i=0;i<nums.length-1;i++){
            arr[i] = nums[i] +nums[i+1];
        }
        
         sumTraingle(arr);
        for(int i=0;i<arr.length;i++){
            System.out.print(arr[i]+" ");
        }
        System.out.println();
    }
}
```
### FirstUppercas
```
class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Try programiz.pro");
      String str = "geeksforGeeKs";
     char ch = firstCapital(str,0);
     System.out.println(ch);
    }
    static char firstCapital(String str, int i){
        if(str.charAt(i) == '\0'){
            return 0;
        }
        if(Character.isUpperCase(str.charAt(i))){
            return str.charAt(i);
        }
        int in =i+1;
        return firstCapital(str,in);
    }
}
```

### Print 1 to N without Loop
```
class HelloWorld {
    public static void main(String[] args) {
       firstCapital(0,10);
    /// System.out.println(ch);
    }
    static int firstCapital( int i,int n){
        if(i==n){
            return i;
        }
        i +=1;
        
        System.out.println(i);
         return firstCapital(i,n);
    }
}

```
### Countnumber of Characters in String
```
class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Try programiz.pro");
        String str = "Gowtham";
        int counter = count(str);
        System.out.println(counter);
    }
    
    static int count(String str){
        if(str.equals("")){
            return 0;
        }
        
        return count(str.substring(1))+1;
    }
}
```
### Geek-onacci Number GFG
```
class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Try programiz.pro");
        int a=1;
        int b=3;
        int c=2;
        int n=6;
        int counter = count(n);
        System.out.println(counter);
    }
    
    static int count(int n){
        if(n==1){
            return 1;
        }
        if(n==2){
            return 3;
        }
        if(n==3){
            return 2;
        }
        
        return count(n-1)+count(n-2)+count(n-3);
    }
}
```
### Sum of digit of a number using Recursion GFG
```
class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Try programiz.pro");
        int n=123456;
        int counter = count(n);
        System.out.println(counter);
    }
    
    static int count(int n){
        if(n==0){
            return 0;
        }
        int num = n/10;
        return count(num)+n%10;
    }
```
