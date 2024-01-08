# java-notes
/**
 * Description:
 *
 * @Author 德
 * @Create 2024/1/8 上午 10:15
 * @Version 1.0
 */
public class compareSelfTest {
    String str1 = "apple";
    String str2 = "banana";


    public void compareStrings() {

        int result = str1.compareTo(str2);

        if (result < 0) {
            System.out.println(str1 + " comes before " + str2);
        } else if (result == 0) {
            System.out.println(str1 + " is equal to " + str2);
        } else {
            System.out.println(str1 + " comes after " + str2);
        }
    }
}

class self extends compareSelfTest{
    public static void main(String[] args) {
        compareSelfTest ct = new compareSelfTest();

        ct.compareStrings();
    }
}
