import javax.swing.*;
import java.awt.*;

/*	2024-10-25
	윈도우 계산기의 버튼 만들기
*/

public class TestM extends JFrame {
    private JTextField display;  // 결과 출력 화면
    private JPanel panel;        // 버튼 패널
    private String[] buttons = { // 버튼 배열
        "%", "CE", "C", "←", "1/x", "x²", "²√x", "÷",
        "7", "8", "9", "×",
        "4", "5", "6", "−",
        "1", "2", "3", "+",
        "+/−", "0", ".", "="
    };

    public TestM() {
        setTitle("계산기");
        setSize(400, 700);
        setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
        setLayout(new BorderLayout());

        // 화면
        display = new JTextField("0");
        display.setEditable(false);
        display.setPreferredSize(new Dimension(400, 100));
        display.setFont(new Font("Arial", Font.PLAIN, 36));
        display.setHorizontalAlignment(SwingConstants.RIGHT);
        add(display, BorderLayout.NORTH);

        // 버튼
        panel = new JPanel();
        panel.setLayout(new GridLayout(6, 4)); // 6행 4열
        for (String text : buttons) {
            JButton button = new JButton(text);
            button.setFont(new Font("Arial", Font.PLAIN, 24));
            panel.add(button);
        }
        add(panel, BorderLayout.CENTER);

        setVisible(true);
    }

    public static void main(String[] args) {
        new TestM();
    }
}
