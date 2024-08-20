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
