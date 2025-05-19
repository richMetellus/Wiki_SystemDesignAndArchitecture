System Design and Project Organization 
#########################################

:date: 05/18/2025

Context 
**********

I was doing some research on strategies to organize complex projects. There are 
many aspects to this: 

1. **Complete Cross-functional project structure**: Do you use a sharepoint,
   share drive to keep important project? - This is more related to project 
   management and product engineering. (not the topic of this journal)
   
   * How do you organize the project in a ways that allows you to share files 
     with internal stakeholders such as system engineers, Electrical engineers, 
     software and also with external suppliers such as contractors, overseas 
     workers.
   
   * This will require people to follow the process outlined by the company.

2. **Code repository|ies structure & management**: What approach do you take to 
   organize code assets in a way that reduce frictions between teams and meet 
   these objectives:

   A. **Easy onboarding**: How easy it is for new developers to be integrated in 
      a team and start contributing to the code base. 
   #. **Visibility & Policy around Access** : How do you control the visibility 
      to a code base? 
      
      For example, in a component-based architecture, how would you structure 
      your repo(s)?

      * if you have an external supplier, how do you limit what he/she can see 
        while having access to the project without limiting?
      
      * Maybe you want that some internal workers that are decision makers to 
        have enough visibility that can help them learn from past failures or 
        success of a project. This should prevent duplicating work, no need to 
        re-invent the wheel.
   
   #. **Re-usability**: how a proven solution, workflow and part of a code base can 
      be re-use across projects. 
   
#. Which architecture pattern is suitable for you application?
   
   A. Monolithic vs Microservices?

This journal article focuses on question 2 & 3. My team at CIM has a large code base 
that use PVCS for version control. They are attempting to move it to GitHub.
The project they said is component based and is re-used on many different 
products. 

The problem: They have been using microcontroller with RTOS and now 
want to go to linux.

1. The CPU architecture are different. i.MX8 (arm, little endian), some product 
   use PowerPC + Renesas RX65N, other product use 2 Renesas RX65N with ThreadX RTOS. 

   Now with the addition of Linux, it's complicated.

2. We need to move the monolithic application codebase from its centrally hosted archive tool 
   PVCS to Github.

   * I researched the Google approach vs Netflix or amazon approach: 
     
     * Google still use Monorepo as legacy code were archived use file-based version 
       control tool. No branching. Google created his own tool Piper for managing 
       its large monorepo.
     
     * Company like Amazon and Netflix has adopted the microservices philosophy. 
       thus this article.
    
    .. seealso:: `Architecture Decomposition (Book ch04)`_ or my copy of the book.

* I have downloaded a series of books on this repo too as I am studying the various 
  approach use in the industries.

References 
***********

.. [#] `How Amazon and Google view CI/CD in an entirely different way`_
.. [#] `Codebase Management | Monorepo vs  Microrepo (LinkedIn)`_
.. [#] `Why Does Google Use Monorepo | Alex Xu`_
.. [#] `How does Google avoid duplicating work? (Quora)`_
.. [#] `Architecture Decomposition (Book ch04)`_

.. include:: ../relevant_urls.rst