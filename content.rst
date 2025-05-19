System Design and Architecture
###################################

**Description and context**

This top parent project is to group relevant topics related to software development 
life cycle from a system designer and architect point of view. 

The goals are to:

1. Help someone knows what make a good system design 
#. To understand what is system architecture and types of systems? 
   
   * distributed systems
     
     * peer-to-peer 
   

#. To understand various kind of software architecture patterns?
   
   * client-server arch 
   * component-base arch 
   * microkernel architecture, event-driven arch. 

    
#. Architectural Styles vs Architectural patterns vs design patterns?
   
   * **design patterns** focuses on code implementation. All architectural 
     pattern are design patterns but not all design patterns are architectural pattern.

     * Client-server is an architectural pattern and might be considered as a 
       design pattern not in the traditional sense of Gang of Four (GoF) design 
       patterns. 
       
       * Ex: Model-View-Control is an architectural pattern and a design pattern. 
       * While client-server is an architectural pattern, you can use various 
         design patterns within it. For example, the Model-View-Controller (MVC) 
         pattern is commonly used in web applications to structure the client-side 
         code. 
    
     * Singleton is a GoF design pattern and not an architectural pattern.
     * GoF design pattern are covered under programming and not here.

**Roadmap**

1. Understand different type of architecture and to what type of application 
   they are suitable?
2. Learn how to implement different type of architectures.
   
   * Learn what make good software design?
   * SOLID principle, GoF design patterns, etc.. 

.. only:: personal

   Journal and Log
   *****************

   .. toctree::
      :caption: Journal
      :glob:
      :numbered:
      :maxdepth: 1

      _Logs_Journal/JNL-*

Courses 
*********

.. toctree::
    :caption: Journal
    :glob:
    :numbered:
    :maxdepth: 1

    Courses/CourseName_git/content