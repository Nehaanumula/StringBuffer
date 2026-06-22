# StringBuffer
Reverse the words in a sentence in java #
class Main{
        StringBuffer sb = new StringBuffer("Hello Hyd");
        String result = "";
        String word = "";
        for (int i = 0; i < sb.length(); i++) {
            char ch = sb.charAt(i);
            if (ch != ' ') {
                word = ch + word;
            } else {
                result = result + word + " ";
                word = "";
            }
        }
        result = result + word;
        System.out.println(result);
    }
}
