# Student-grade-calculator-
public  class Main {
    public static void main(String[] args) {
        System.out.println("this application is calculate students marks,average percentage,grad calculation");
        Scanner scanner=new Scanner(System.in);
   System.out.println("please enter the total subject:");
        int subject=scanner.nextInt();//user through input as total subject
        int total_marks=0;//
        for(int i=0;i<subject;i++){
            System.out.println("please enter the each subject marks:");
         int marks=scanner.nextInt();
         total_marks=total_marks+marks;
        }
        float Percentage = total_marks / subject;
        char grade = 0;
        if(Percentage>90){
            grade ='A';
        } else if (Percentage>=80 && Percentage <=90) {
            grade ='B';
        }else if(Percentage>=70 && Percentage<=80){
            grade ='C';
        }else if(Percentage>=60 && Percentage<=70){
            grade ='D';
        }else if(Percentage>=50 && Percentage<=60){
            grade ='E';
        }else if(Percentage>=40 && Percentage<=50){
            grade ='F';
        }else{
            System.out.println("you fail in the exam better luck next time:");
        }
        System.out.println("your total marks is:"+total_marks);
        System.out.println("your percentage is:"+Percentage+"%");
        System.out.println("your grade is:"+grade);
    }

}
