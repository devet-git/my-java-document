# This is example about how to use ArrayList in Java 

```java

import java.util.ArrayList;

//TODO: declare class User
class User {
   private String id;
   private String fullName;
   private String username;
   private String password;
   
   public User(String id, String fullName, String username, String password) {
      this.id = id;
      this.fullName = fullName;
      this.username = username;
      this.password = password;
   }
   
   public String getId() {
      return id;
   }
   
   public void setId(String id) {
      this.id = id;
   }
   
   public String getFullName() {
      return fullName;
   }
   
   public void setFullName(String fullName) {
      this.fullName = fullName;
   }
   
   public String getUsername() {
      return username;
   }
   
   public void setUsername(String username) {
      this.username = username;
   }
   
   public String getPassword() {
      return password;
   }
   
   public void setPassword(String password) {
      this.password = password;
   }
}


public class ArrayListExample {
   
  //TODO: declare User ArrayList 
   ArrayList<User> users =new ArrayList<>();
   {
      users.add(new User("1", "Thang", "thangq1", "12345678"));
      users.add(new User("2", "Thang", "thangq2", "12345678"));
      users.add(new User("3", "Thang", "thangq3", "12345678"));
      users.add(new User("4", "Thang", "thangq4", "12345678"));
   }
   
   public void main(String[] args){
      String userId = "2";
     
      //TODO: loop over araylist
      for (User u : this.users) {
         //TODO: find item by id
         if (u.getId().equals(userId)) {
            users.remove(u); //TODO: remove item from arraylist
         }
      }
   }
}

```
