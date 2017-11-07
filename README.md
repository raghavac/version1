import java.awt.*;
import java.awt.event.*;
import javax.swing.*;
import org.jdesktop.layout.GroupLayout;
import org.jdesktop.layout.LayoutStyle;
public class login extends JFrame {
	public login() {
		initComponents();
	}

	private void button1ActionPerformed(ActionEvent e) {
	}

	private void initComponents() {
		window1 = new Window();
		label1 = new JLabel();
		label2 = new JLabel();
		textField1 = new JTextField();
		textField2 = new JTextField();
		button1 = new JButton();
		{
			label1.setText("UserName");
			label2.setText("Password");
			button1.setText("Login");
			button1.addActionListener(new ActionListener() {
				public void actionPerformed(ActionEvent e) {
					button1ActionPerformed(e);
				}
			});

			GroupLayout window1Layout = new GroupLayout(window1);
			window1.setLayout(window1Layout);
			window1Layout.setHorizontalGroup(
				window1Layout.createParallelGroup()
					.add(window1Layout.createSequentialGroup()
						.add(24, 24, 24)
						.add(window1Layout.createParallelGroup()
							.add(label2)
							.add(label1))
						.add(18, 18, 18)
						.add(window1Layout.createParallelGroup()
							.add(textField1, GroupLayout.DEFAULT_SIZE, 171, Short.MAX_VALUE)
							.add(textField2))
						.add(13, 13, 13))
					.add(GroupLayout.TRAILING, window1Layout.createSequentialGroup()
						.addContainerGap(126, Short.MAX_VALUE)
						.add(button1)
						.add(92, 92, 92))
			);
			window1Layout.setVerticalGroup(
				window1Layout.createParallelGroup()
					.add(window1Layout.createSequentialGroup()
						.add(45, 45, 45)
						.add(window1Layout.createParallelGroup(GroupLayout.BASELINE)
							.add(label1)
							.add(textField1, GroupLayout.PREFERRED_SIZE, GroupLayout.DEFAULT_SIZE, GroupLayout.PREFERRED_SIZE))
						.add(18, 18, 18)
						.add(window1Layout.createParallelGroup()
							.add(label2)
							.add(textField2, GroupLayout.PREFERRED_SIZE, GroupLayout.DEFAULT_SIZE, GroupLayout.PREFERRED_SIZE))
						.add(30, 30, 30)
						.add(button1)
						.addContainerGap(44, Short.MAX_VALUE))
			);
			window1.pack();
			window1.setLocationRelativeTo(window1.getOwner());
		}
		// JFormDesigner - End of component initialization  //GEN-END:initComponents
	}

	// JFormDesigner - Variables declaration - DO NOT MODIFY  //GEN-BEGIN:variables
	// Generated using JFormDesigner Evaluation license - chilamathur raghavendra
	private Window window1;
	private JLabel label1;
	private JLabel label2;
	private JTextField textField1;
	private JTextField textField2;
	private JButton button1;
	// JFormDesigner - End of variables declaration  //GEN-END:variables
}
