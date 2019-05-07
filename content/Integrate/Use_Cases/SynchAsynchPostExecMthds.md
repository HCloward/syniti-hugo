+++
title = 'Synchronous and Asynchronous Post Execution Methods'
solution = 'Platform'
+++

# Synchronous and Asynchronous Post Execution Methods

Integrate supports two types of Post Execution Methods for a process:
Synchronous and Asynchronous. 

Using the asynchronous method, Integrate posts data using a two-stage
process when interacting with the target system. First, Integrate sends
data to the target system, which processes the data. Second, Integrate
then polls the target system for the posting status. When a process is
added, the default post execution method is asynchronous.

The synchronous post execution method sends data to the target system
and waits for a response for each record before posting the next
record.  Template types BDC Script, GUI Script, and BAPI/RFC can use
the synchronous post execution method.

Set the post execution method at the process level when adding or
editing a process. On the *Process* page’s *Vertical* View, on the
**Advanced** tab, select an option in the **Post Execution Method** list
box. Refer to *<span style="color: #0000ff;font-style: normal;">[Create
a Process](Create_a_Process.htm)</span>* for more information.
