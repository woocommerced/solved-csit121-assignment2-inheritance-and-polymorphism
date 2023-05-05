Download Link: https://assignmentchef.com/product/solved-csit121-assignment2-inheritance-and-polymorphism
<br>
This assignment aims to provide you with some experience in writing codes using Java programming language that covers the following topics:

<ul>

 <li>Inheritance and Polymorphism</li>

 <li>Object Interactions</li>

</ul>

<table width="732">

 <tbody>

  <tr>

   <td width="732"><strong> </strong><strong>Remember that: </strong><strong>1.         </strong><strong>All programs should be able to run on the lab’s computers. </strong><strong>2.         </strong><strong>You must put the following information on the header of each text and source file you will be submitting in this assignment:  </strong><strong>     Student’s full name:   </strong><strong>     Student’s ID:   </strong><strong>     Modification Date:  </strong><strong>     Purpose of this file (or program):   </strong><strong>3.         </strong><strong>Assignments that are not able to be compiled will result in zero mark given to the assignment. </strong><strong>4.         </strong><strong>You must only use the Java features that have already been covered in the lectures </strong><strong> </strong></td>

  </tr>

 </tbody>

</table>




<strong>Question: </strong>




A resort near Pangkor Island offers rental items to their customers at a price. The customer may rent a number of rental items which can include a boat, a bicycle, or a jet ski. You are required to write a Java application that keeps track of the items rented by each customer and also able to calculate the total rental amount due.




To implement this, you need to declare several classes. The classes includes the RentalItem class which is inherited by the Boat class, the Bicycle class, and the JetSki class. A Customer class is also required to keep track of the customers renting the items. Lastly, you also need another class called Rental that will relate the Customer object with a number of RentalItem object.




The classes are partially described in the following diagrams:

The RentalItem class and its subclasses.




<table width="306">

 <tbody>

  <tr>

   <td width="306"><em>abstract RentalItem </em></td>

  </tr>

  <tr>

   <td width="306"></td>

  </tr>

  <tr>

   <td width="306">+ RentalItem()+ RentalItem(int,double,int)<em>+ calculateRental() : double </em>//necessary get and set methods</td>

  </tr>

 </tbody>

</table>




Include the necessary accessors and mutators to the classes. The calculateRental() method should perform different calculation to get the rental amount for each object. The calculation is as follows:







<table width="654">

 <tbody>

  <tr>

   <td width="132">Boat</td>

   <td width="522">Rental is calculated based on capacity. A boat for 10 passengers and more is charged with the rate per day plus additional charges of RM50 and a boat for less than 10 passengers has no additional charges. </td>

  </tr>

  <tr>

   <td width="132">Bicycle</td>

   <td width="522">A mountain bike has additional charges of RM10 than the normal rate per day.A kids bike is given half the price of the normal rate per day. Other bikes are charged at the normal rate. </td>

  </tr>

  <tr>

   <td width="132">JetSki</td>

   <td width="522">A jet ski with 250 horse power or below has no additional charge. Others will be charged at 1.5 of the normal rate. </td>

  </tr>

 </tbody>

</table>




The Customer class.

<strong> </strong>

<table width="306">

 <tbody>

  <tr>

   <td width="306"></td>

  </tr>

  <tr>

   <td width="306">–  name : String–  contactNo : String</td>

  </tr>

  <tr>

   <td width="306">+ Customer(String,String)//necessary get and set methods</td>

  </tr>

 </tbody>

</table>

<strong> </strong>

The Rental Class







<table width="348">

 <tbody>

  <tr>

   <td width="348"></td>

  </tr>

  <tr>

   <td width="348">–  id : int–  customer : Customer–  rentalItems : ArrayList&lt;RentalItem&gt;</td>

  </tr>

  <tr>

   <td width="348">+ Rental()+ setCustomer() : void+ addRentalItem(RentalItem) : void+ removeRentalItem() : void+ calculateTotalRental() : double</td>

  </tr>

 </tbody>

</table>










The Rental class will include the object of class Customer and an ArrayList of RentalItem objects.




The rentalItems ArrayList should be declared as RentalItem type so that it can store any number of objects from different subclasses of RentalItem class (either Boat, Bicycle, or JetSki). Each customer can rent as many of these items as they wish.




The addRentalItem(RentalItem) method should receive a RentalItem object and add it to the ArrayList. The calculateTotalRental() method should add the rental amount from each rental items and return the value.







Lastly, write a main() method that keeps several Rental objects. Use suitable menu driven application to allow the user to add customer, add rental items, remove rental items, display all rental details and total rental charges, and display a single rental details and its total charges.




You are required to ensure that all errors are handled properly. Use exception handling technique and/or condition validation as necessary. Include meaningful comments in your programs and make your programs readable. Be creative in displaying your outputs.













<strong> </strong>


