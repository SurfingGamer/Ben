if (event.getSource() instanceof JMenuItem){    
            JMenuItem jmi = (JMenuItem) event.getSource();
            JPopupMenu jpm = (JPopupMenu) jmi.getParent();
            JMenu menuChoice = (JMenu) jpm.getInvoker();
            if(menuChoice.getText().equals("Add")){
                if (jmi.getText().equals("Client")){
                    AddClient ac = new AddClient();
                    this.dispose();
                }
                if (jmi.getText().equals("DVD")){
                    AddDVD ad = new AddDVD();
                    this.dispose();
                }
                if (jmi.getText().equals("User")){
                    AddUser au = new AddUser();
                    this.dispose();
                } 
            }
            if (menuChoice.getText().equals("Edit")){
                if(jmi.getText().equals("Client")){
                    EditClient ec = new EditClient();
                    this.dispose();
                }
                if (jmi.getText().equals("DVD")){
                    EditDVD ed = new EditDVD();
                    this.dispose();
                }
                if (jmi.getText().equals("User")){
                    EditUser eu = new EditUser();
                    this.dispose();
                } 
            }
