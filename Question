package JavaProject;
import javax.swing.*;
import java.sql.*;
public class Questions extends javax.swing.JFrame {

    static int count=0,flag=0,sum=0; 
    int QNO=1;
    static int option=Topics.topic;
    
    public Questions() {
        setResizable(false);
        setTitle("Welcome to Knowledge Testing Portal");
        setLocation(600,250);
        initComponents();
        if(option==1){
            Computer_question();  
        }
        else if(option==2){
            Reasoning_question();  
        }
        else if(option==3){
            English_question();
        }
        else if(option==4){
            General_knowledge_question();
        }         
    }
    
    void Computer_question()
    {
        PreparedStatement ps;
        ResultSet rs;
        String query = "SELECT ques_no,ques,option1,option2,option3,option4,correct FROM computer WHERE ques_no="+QNO;
        try {
         
            ps =  connection_established.getConnection().prepareStatement(query);
            rs=ps.executeQuery();
            while(rs.next())
            {  
                text_area.setText(rs.getInt("ques_no")+". "+rs.getString("ques"));
                option1_.setText(rs.getString("option1"));
                option2_.setText(rs.getString("option2"));
                option3_.setText(rs.getString("option3"));
                option4_.setText(rs.getString("option4"));
                answer.setText(rs.getString("correct"));
                answer.setVisible(false);
            }
            rs.close();
        } catch (SQLException ex) {
               JOptionPane.showMessageDialog(null,ex);
        }
        
    }
    
    void Reasoning_question(){
   
        PreparedStatement ps;
        ResultSet rs;
        String query = "SELECT ques_no,ques,option1,option2,option3,option4,correct FROM reasoning WHERE ques_no="+QNO;
        try {
            ps =  connection_established.getConnection().prepareStatement(query);
            rs=ps.executeQuery();
            while(rs.next())
            {
                text_area.setText(rs.getInt("ques_no")+". "+rs.getString("ques"));
                option1_.setText(rs.getString("option1"));
                option2_.setText(rs.getString("option2"));
                option3_.setText(rs.getString("option3"));
                option4_.setText(rs.getString("option4"));
                answer.setText(rs.getString("correct"));
                answer.setVisible(false);
            }
            rs.close();
        } catch (SQLException ex) {
               JOptionPane.showMessageDialog(null,ex);
        }
    }
    
    void English_question(){
        
        PreparedStatement ps;
        ResultSet rs;
        String query = "SELECT ques_no,ques,option1,option2,option3,option4,correct FROM english WHERE ques_no="+QNO;
        try {
         
            ps =  connection_established.getConnection().prepareStatement(query);
            rs=ps.executeQuery();
            while(rs.next())
            {
                text_area.setText(rs.getInt("ques_no")+". "+rs.getString("ques"));
                option1_.setText(rs.getString("option1"));
                option2_.setText(rs.getString("option2"));
                option3_.setText(rs.getString("option3"));
                option4_.setText(rs.getString("option4"));
                answer.setText(rs.getString("correct"));
                answer.setVisible(false);
            }
            rs.close();
        } catch (SQLException ex) {
               JOptionPane.showMessageDialog(null,ex);
        }
    }
    
    void General_knowledge_question(){
        
        PreparedStatement ps;
        ResultSet rs;
        String query = "SELECT ques_no,ques,option1,option2,option3,option4,correct FROM gk WHERE ques_no="+QNO;
        try {
         
            ps =  connection_established.getConnection().prepareStatement(query);
            rs=ps.executeQuery();
            while(rs.next()){
                
                text_area.setText(rs.getInt("ques_no")+". "+rs.getString("ques"));
                option1_.setText(rs.getString("option1"));
                option2_.setText(rs.getString("option2"));
                option3_.setText(rs.getString("option3"));
                option4_.setText(rs.getString("option4"));
                answer.setText(rs.getString("correct"));
                answer.setVisible(false);
            }
            rs.close();
        } catch (SQLException ex) {
               JOptionPane.showMessageDialog(null,ex);
        }
    }
    
    @SuppressWarnings("unchecked")
    // <editor-fold defaultstate="collapsed" desc="Generated Code">//GEN-BEGIN:initComponents
    private void initComponents() {

        buttonGroup1 = new javax.swing.ButtonGroup();
        jScrollPane1 = new javax.swing.JScrollPane();
        text_area = new javax.swing.JTextArea();
        option1_ = new javax.swing.JRadioButton();
        option2_ = new javax.swing.JRadioButton();
        option3_ = new javax.swing.JRadioButton();
        option4_ = new javax.swing.JRadioButton();
        next_question = new javax.swing.JButton();
        logout = new javax.swing.JButton();
        answer = new javax.swing.JLabel();
        Final_submition = new javax.swing.JButton();
        jPanel2 = new javax.swing.JPanel();
        jPanel3 = new javax.swing.JPanel();

        buttonGroup1.add(option1_);
        buttonGroup1.add(option2_);
        buttonGroup1.add(option3_);
        buttonGroup1.add(option4_);

        setDefaultCloseOperation(javax.swing.WindowConstants.EXIT_ON_CLOSE);
        setBackground(new java.awt.Color(255, 255, 225));
        setCursor(new java.awt.Cursor(java.awt.Cursor.DEFAULT_CURSOR));
        getContentPane().setLayout(new org.netbeans.lib.awtextra.AbsoluteLayout());

        text_area.setBackground(new java.awt.Color(255, 153, 255));
        text_area.setColumns(20);
        text_area.setFont(new java.awt.Font("Times New Roman", 1, 24)); // NOI18N
        text_area.setForeground(new java.awt.Color(0, 0, 255));
        text_area.setRows(5);
        jScrollPane1.setViewportView(text_area);

        getContentPane().add(jScrollPane1, new org.netbeans.lib.awtextra.AbsoluteConstraints(70, 30, 790, 200));

        option1_.setBackground(new java.awt.Color(0, 255, 102));
        option1_.setFont(new java.awt.Font("Times New Roman", 1, 18)); // NOI18N
        option1_.setForeground(new java.awt.Color(255, 0, 0));
        option1_.setText("Option1");
        option1_.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                option1_ActionPerformed(evt);
            }
        });
        getContentPane().add(option1_, new org.netbeans.lib.awtextra.AbsoluteConstraints(161, 249, 250, 50));

        option2_.setBackground(new java.awt.Color(0, 255, 102));
        option2_.setFont(new java.awt.Font("Times New Roman", 1, 18)); // NOI18N
        option2_.setForeground(new java.awt.Color(255, 0, 0));
        option2_.setText("Option2");
        option2_.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                option2_ActionPerformed(evt);
            }
        });
        getContentPane().add(option2_, new org.netbeans.lib.awtextra.AbsoluteConstraints(510, 249, 260, 50));

        option3_.setBackground(new java.awt.Color(0, 255, 102));
        option3_.setFont(new java.awt.Font("Times New Roman", 1, 18)); // NOI18N
        option3_.setForeground(new java.awt.Color(255, 0, 0));
        option3_.setText("Option3");
        getContentPane().add(option3_, new org.netbeans.lib.awtextra.AbsoluteConstraints(161, 327, 250, 50));

        option4_.setBackground(new java.awt.Color(0, 255, 102));
        option4_.setFont(new java.awt.Font("Times New Roman", 1, 18)); // NOI18N
        option4_.setForeground(new java.awt.Color(255, 0, 0));
        option4_.setText("Option4");
        option4_.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                option4_ActionPerformed(evt);
            }
        });
        getContentPane().add(option4_, new org.netbeans.lib.awtextra.AbsoluteConstraints(510, 327, 260, 50));

        next_question.setBackground(new java.awt.Color(0, 0, 255));
        next_question.setFont(new java.awt.Font("Times New Roman", 1, 24)); // NOI18N
        next_question.setForeground(new java.awt.Color(255, 255, 255));
        next_question.setText("Next ");
        next_question.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                next_questionActionPerformed(evt);
            }
        });
        getContentPane().add(next_question, new org.netbeans.lib.awtextra.AbsoluteConstraints(80, 450, 190, 70));

        logout.setBackground(new java.awt.Color(255, 0, 51));
        logout.setFont(new java.awt.Font("Times New Roman", 1, 24)); // NOI18N
        logout.setForeground(new java.awt.Color(255, 255, 255));
        logout.setText("EXIT");
        logout.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                logoutActionPerformed(evt);
            }
        });
        getContentPane().add(logout, new org.netbeans.lib.awtextra.AbsoluteConstraints(650, 450, 190, 70));

        answer.setText("Ans");
        getContentPane().add(answer, new org.netbeans.lib.awtextra.AbsoluteConstraints(20, 480, 30, -1));

        Final_submition.setBackground(new java.awt.Color(0, 255, 0));
        Final_submition.setFont(new java.awt.Font("Times New Roman", 1, 24)); // NOI18N
        Final_submition.setForeground(new java.awt.Color(255, 255, 255));
        Final_submition.setText("Submit");
        Final_submition.addActionListener(new java.awt.event.ActionListener() {
            public void actionPerformed(java.awt.event.ActionEvent evt) {
                Final_submitionActionPerformed(evt);
            }
        });
        getContentPane().add(Final_submition, new org.netbeans.lib.awtextra.AbsoluteConstraints(370, 450, 170, 70));

        jPanel2.setBackground(new java.awt.Color(138, 209, 255));
        getContentPane().add(jPanel2, new org.netbeans.lib.awtextra.AbsoluteConstraints(0, 420, 940, 140));

        jPanel3.setBackground(new java.awt.Color(153, 0, 153));
        getContentPane().add(jPanel3, new org.netbeans.lib.awtextra.AbsoluteConstraints(-10, 0, 950, 420));

        pack();
    }// </editor-fold>//GEN-END:initComponents

    private void next_questionActionPerformed(java.awt.event.ActionEvent evt) {//GEN-FIRST:event_next_questionActionPerformed

        if(option==1){
            
            if(QNO<=10){    
                //**************************************** for 1 to 10 computer question *********************

                String opt1="";
                String ans=answer.getText();
                if(option1_.isSelected()){
                    opt1=option1_.getText();
                }
                else if(option2_.isSelected()){
                    opt1=option2_.getText();
                }
                else if(option3_.isSelected()){
                    opt1=option3_.getText();
                }
                else if(option4_.isSelected()){
                    opt1=option4_.getText();
                }

                //If selected option is matched with correct answer.
                if(opt1.equals(ans)){
                    count++;
                    buttonGroup1.clearSelection(); //Clears the selection such that none of the buttons in the ButtonGroup are selected.
                }
                //If user has not selected any option and press next button.
                else if(!option1_.isSelected()&&!option2_.isSelected()&&!option3_.isSelected()&&!option4_.isSelected()){
                    sum++;    
                }
                //If selected option does not match with correct answer.
                else {
                    flag++;
                    buttonGroup1.clearSelection();
                }

                QNO++;   
                Computer_question();
            }
            else{
                QNO=1;
            }           
        }
        
        else if(option==2){
        
            if(QNO<=10){    
                //**************************************** for 1 to 10 Reasoning question *********************//
                String opt1="";
                String ans=answer.getText();
                if(option1_.isSelected()){
                    opt1=option1_.getText();
                }
                else if(option2_.isSelected()){
                    opt1=option2_.getText();
                }
                else if(option3_.isSelected()){
                    opt1=option3_.getText();
                }
                else if(option4_.isSelected()){
                    opt1=option4_.getText();
                }

                //If selected option is matched with correct answer.
                if(opt1.equals(ans)){
                    count++;
                    buttonGroup1.clearSelection();
                }
                //If user has not selected any option and press next button.
                else if(!option1_.isSelected()&&!option2_.isSelected()&&!option3_.isSelected()&&!option4_.isSelected()){
                    sum++;  
                }
                //If selected option does not match with correct answer.
                else{
                    flag++;
                    buttonGroup1.clearSelection();
                }

                QNO++;   
                //System.out.println(count);
                Reasoning_question();
            }
            
            else{
                QNO=1;
            }           
        }
    
        else if(option==3){

            if(QNO<=10){    
                //**************************************** for 1 to 10 English question *********************
   
                String opt1="";
                String ans=answer.getText();
                if(option1_.isSelected()){
                    opt1=option1_.getText();
                }
                else if(option2_.isSelected()){
                    opt1=option2_.getText();
                }
                else if(option3_.isSelected()){
                    opt1=option3_.getText();
                }
                else if(option4_.isSelected()){
                    opt1=option4_.getText();
                }

                //If selected option is matched with correct answer.
                if(opt1.equals(ans)){
                    count++;
                    buttonGroup1.clearSelection();
                }
                //If user has not selected any option and press next button.
                else if(!option1_.isSelected()&&!option2_.isSelected()&&!option3_.isSelected()&&!option4_.isSelected()){
                    sum++;  
                }
                //If selected option does not match with correct answer.
                else {
                    flag++;
                    buttonGroup1.clearSelection();
                }

                QNO++;   
                English_question();
            }
            else{
                QNO=1;
            }           
        }
   
        else if(option==4){
        
            if(QNO<=10){    
                // **************************************** for 1 to 10 General Kowledge question *********************
   
                String opt1="";
                String ans=answer.getText();
                if(option1_.isSelected()){
                    opt1=option1_.getText();
                }
                else if(option2_.isSelected()){
                    opt1=option2_.getText();
                }
                else if(option3_.isSelected()){
                    opt1=option3_.getText();
                }
                else if(option4_.isSelected()){
                    opt1=option4_.getText();
                }
                
                //If selected option is matched with correct answer.
                if(opt1.equals(ans)){   
                    count++;
                    buttonGroup1.clearSelection();
                }
                //If user has not selected any option and press next button.
                else if(!option1_.isSelected()&&!option2_.isSelected()&&!option3_.isSelected()&&!option4_.isSelected()){
                    sum++;  
                }
                
                //If selected option does not match with correct answer.
                else{
                    flag++;
                    buttonGroup1.clearSelection();
                }
                
                QNO++;   
                General_knowledge_question();
            }
            else{
                QNO=1;
            }           
        }
        
        if((sum+flag+count)==10){
          
            JOptionPane.showMessageDialog(null,"End Question Press the Submit Button And check your score");
        }
                                   
    }//GEN-LAST:event_next_questionActionPerformed
  
    private void logoutActionPerformed(java.awt.event.ActionEvent evt) {//GEN-FIRST:event_logoutActionPerformed
        
        JOptionPane.showMessageDialog(null, "You have now left the test.");
        System.exit(0);
    }//GEN-LAST:event_logoutActionPerformed

    private void option2_ActionPerformed(java.awt.event.ActionEvent evt) {//GEN-FIRST:event_option2_ActionPerformed
        // TODO add your handling code here:
    }//GEN-LAST:event_option2_ActionPerformed

    private void option4_ActionPerformed(java.awt.event.ActionEvent evt) {//GEN-FIRST:event_option4_ActionPerformed
        // TODO add your handling code here:
    }//GEN-LAST:event_option4_ActionPerformed

    private void Final_submitionActionPerformed(java.awt.event.ActionEvent evt) {//GEN-FIRST:event_Final_submitionActionPerformed
        
        this.dispose();
        ScoreBoard t= new ScoreBoard();
        t.setVisible(true);
        flag=0;
        count=0;
        sum=0;    
    }//GEN-LAST:event_Final_submitionActionPerformed

    private void option1_ActionPerformed(java.awt.event.ActionEvent evt) {//GEN-FIRST:event_option1_ActionPerformed
        // TODO add your handling code here:
    }//GEN-LAST:event_option1_ActionPerformed

   
    public static void main(String args[]) {
        
        new Questions().setVisible(true);
    }
  
    // Variables declaration - do not modify//GEN-BEGIN:variables
    private javax.swing.JButton Final_submition;
    private javax.swing.JLabel answer;
    private javax.swing.ButtonGroup buttonGroup1;
    private javax.swing.JPanel jPanel2;
    private javax.swing.JPanel jPanel3;
    private javax.swing.JScrollPane jScrollPane1;
    private javax.swing.JButton logout;
    private javax.swing.JButton next_question;
    private javax.swing.JRadioButton option1_;
    private javax.swing.JRadioButton option2_;
    private javax.swing.JRadioButton option3_;
    private javax.swing.JRadioButton option4_;
    private javax.swing.JTextArea text_area;
    // End of variables declaration//GEN-END:variables
}
