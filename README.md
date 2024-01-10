# Patient-Triage-System
This Java application implements a patient triage system using a priority queue based on a heap data structure. The system is designed to prioritize patients based on their condition or age, depending on the chosen comparator.

Components
Heap
The Heap class implements the priority queue and heap functionality. It supports both max and min heaps, and users can choose the sorting order by providing a comparator. The heap operations such as enqueueElement, dequeueElement, bubbleUp, and bubbleDown ensure that the heap properties are maintained.

AppMain
The AppMain class serves as the main entry point for the application. It reads patient information from a file using TriageSystemParser, creates a priority queue using the Heap class, and enqueues patients based on their conditions or ages. The application then dequeues and prints the patients, demonstrating the functionality of the triage system.

TriageSystemParser
The TriageSystemParser class is responsible for reading patient information from a file. It uses this information to create a list of Patient objects.

Patient
The Patient class represents a patient with attributes such as name, condition, and age. It is used in conjunction with comparators to determine priority in the triage system.

Comparators
Two comparators, PatientConditionComparator and PatientAgeComparator, are provided for sorting patients based on their conditions or ages. Users can easily switch between them to change the priority criteria.
