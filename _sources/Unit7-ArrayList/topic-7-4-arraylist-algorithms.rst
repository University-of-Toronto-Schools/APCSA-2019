.. qnum::
   :prefix: 7-4-
   :start: 1

.. |CodingEx| image:: ../../_static/codingExercise.png
    :width: 30px
    :align: middle
    :alt: coding exercise
    
    
.. |Exercise| image:: ../../_static/exercise.png
    :width: 35
    :align: middle
    :alt: exercise
    
    
.. |Groupwork| image:: ../../_static/groupwork.png
    :width: 35
    :align: middle
    :alt: groupwork
    
ArrayList Algorithms
=====================
   
There are standard ArrayList algorithms that utilize traversals to:

  - Insert elements
  - Delete elements
  - Determine the minimum or maximum value 
  - Compute a sum, average, or mode of elements
  - Search for a particular element in the array
  - Determine if at least one element has a particular property
  - Determine if all elements have a particular property
  - Access all consecutive pairs of elements
  - Determine the presence or absence of duplicate elements
  - Determine the number of elements meeting specific criteria
  - Shift or rotate elements left or right
  - Reverse the order of the elements

Here are two common ArrayList traversal loops that can be used for these algorithms:

.. code-block:: java 
 

  for (Type obj : list)
  {
      if (obj ....)
          ...
  }
  
  for(int i=0; i < list.size(); i++) 
  {
     if (list.get(i) ....)
         ...
  }  
  
You should be able to trace through code that uses all the basic ArrayList methods like the following.

|Exercise| **Check Your Understanding**

.. mchoice:: qListRem3
   :answer_a: [1, 2, 3, 4, 5]
   :answer_b: [1, 2, 4, 5, 6]
   :answer_c: [1, 2, 5, 4, 6]
   :answer_d: [1, 5, 2, 4, 6]
   :correct: d
   :feedback_a: The <code>set</code> will replace the 3 at index 2 so this isn't correct.
   :feedback_b: The <code>add</code> with an index of 1 and a value of 5 adds the 5 at index 1 not 3. Remember that the first index is 0.
   :feedback_c: The <code>set</code> will change the item at index 2 to 4.  The <code>add</code> of 5 at index 1 will move everything else to the right and insert 5.  The last <code>add</code> will be at the end of the list.
   :feedback_d: <code>add</code> without an index adds at the end, <code>set</code> will replace the item at that index, <code>add</code> with an index will move all current values at that index or beyond to the right.
  
   What will print when the following code executes?
   
   .. code-block:: java
   
      List<Integer> numList = new ArrayList<Integer>();
      numList.add(new Integer(1));
      numList.add(new Integer(2));
      numList.add(new Integer(3));
      numList.set(2,new Integer(4));
      numList.add(1, new Integer(5));
      numList.add(new Integer(6));
      System.out.println(numList);
      
You can step through the code above by clicking on the following `Example1 <http://cscircles.cemc.uwaterloo.ca/java_visualize/#code=import+java.util.*%3B%0A%0Apublic+class+ClassNameHere+%7B%0A+++public+static+void+main(String%5B%5D+args)+%7B%0A++++++%0A++++++List%3CInteger%3E+list1+%3D+new+ArrayList%3CInteger%3E()%3B%0A++++++list1.add(new+Integer(1))%3B%0A++++++System.out.println(list1)%3B%0A++++++list1.add(new+Integer(2))%3B%0A++++++System.out.println(list1)%3B%0A++++++list1.add(new+Integer(3))%3B%0A++++++System.out.println(list1)%3B%0A++++++list1.set(2,+new+Integer(4))%3B%0A++++++System.out.println(list1)%3B%0A++++++list1.add(1,+new+Integer(5))%3B%0A++++++System.out.println(list1)%3B%0A++++++list1.add(new+Integer(6))%3B%0A++++++System.out.println(list1)%3B%0A++++++%0A+++%7D%0A%7D&mode=display&curInstr=0>`_.
      
.. mchoice:: qListRem4
   :answer_a: [2, 3]
   :answer_b: [1, 2, 3]
   :answer_c: [1, 2]
   :answer_d: [1, 3]
   :correct: d
   :feedback_a: The <code>remove</code> will remove the item at the given index.  
   :feedback_b: The item at index 1 will be removed and all the other values shifted left.
   :feedback_c: The 3 is at index 2.  The item at index 1 will be removed. 
   :feedback_d: The item at index 1 is removed and the 3 is moved left.  

   What will print when the following code executes?
   
   .. code-block:: java 
   
      List<Integer> list1 = new ArrayList<Integer>();
      list1.add(new Integer(1));
      list1.add(new Integer(2));
      list1.add(new Integer(3));
      list1.remove(1);
      System.out.println(list1);
      
You can step through the code above by clicking on the following `Example2 <http://cscircles.cemc.uwaterloo.ca/java_visualize/#code=import+java.util.*%3B%0A%0Apublic+class+ClassNameHere+%7B%0A+++public+static+void+main(String%5B%5D+args)+%7B%0A++++++List%3CInteger%3E+list1+%3D+new+ArrayList%3CInteger%3E()%3B%0A++++++list1.add(new+Integer(1))%3B%0A++++++System.out.println(list1)%3B%0A++++++list1.add(new+Integer(2))%3B%0A++++++System.out.println(list1)%3B%0A++++++list1.add(new+Integer(3))%3B%0A++++++System.out.println(list1)%3B%0A++++++list1.remove(1)%3B%0A++++++System.out.println(list1)%3B%0A+++%7D%0A%7D&mode=display&curInstr=0>`_.


Some algorithms require multiple String, array, or ArrayList objects to be traversed simultaneously.
      

We encourage you to work in pairs or groups to tackle the following challenging FRQ problems and take them one step at a time. These will get easier with practice! 

.. toctree::
   :maxdepth: 3

   stringScrambleB.rst
   climbClubA.rst
   climbClubB.rst
   climbClubC.rst
   cookieOrderA.rst
   cookieOrderB.rst
   2016freeresponseQ4A.rst
   2016freeresponseQ4B.rst
      
