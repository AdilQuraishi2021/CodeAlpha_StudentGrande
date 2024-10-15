import java.util.ArrayList;
import java.util.List;
import java.util.Scanner;

class StudentGradeTracker{
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        List<Float> grades = new ArrayList<>();
        boolean flag = true;
        System.out.println("Enter grades or -1 to stop entry: ");
        double sum =0;
        while (flag) {
            float val = sc.nextFloat();
            if(val == -1)
                break;
            grades.add(val);
            sum += val;
        }
        float avg = (float)sum/grades.size();
        float highest = Float.MAX_VALUE;
        float lowest = Float.MAX_VALUE;
        for(float grade : grades){
            if(grade > highest)
                highest = grade;
            if (grade < lowest) 
                lowest = grade;
        }
        System.out.println("Average : "+ avg);
        System.out.println("Highest : "+ (grades.size() == 0?0:highest));
        System.out.println("Lowest : "+ (grades.size() == 0?0:lowest));
        }
}
