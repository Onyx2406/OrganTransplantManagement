# OrganTransplantManagement

The program searches through all possible matches with the same organ
and blood type. It calculates a score for each patient based on the time the
patient has been waiting (their location in the list) and the patient's
survivability. However, it only looks at patients who live close enough to the
donor such that the organ can be transplanted to the patient before the
patient passes away.
A graph of Indian cities is used to determine this and a searching algorithm
is used to determine the shortest path between the donor's city and the
patient's city. If a match is found when a donor or patient is added, the pair
is added to a queueThe user can then select "Operate", which will operate on the first pair in
the queue and determine if the operation was a success depending on the
patient's likelihood of survivability. The user can print the matches waiting
to be operated on. They can also print the patients and donors waiting for a
match. The user can also count the patients and the donors waiting for a
match.

Options Implemented
1. Add a patient: When prompted, the user will enter the patient's name,
organ needed, blood type, chance of survivability, time left, and location.
The name should be the patient's last name. The organ needed can be
heart, lungs, liver, pancreas, kidney, intestines, or head, and must not be
capitalized. The blood type can be O, A, B, or AB, and must be capitalized.
Chance of survivability should be between 0 and 100. Time left should be in
hours.

2. Add a donor: Same as adding a patient, but the user will not be
prompted for survivability or time left since those attributes do not apply to
donors.

3. Delete a patient: User will be prompted for the patient's name. It
should be their last name.

4. Delete a donor: Same as delete patient. For example: "Benson".

5. Count patients: This will count the number of patients waiting and
output the number. It does not require any input arguments.

6. Count donors: This will count the number of donors waiting and output
the number. It does not require any input arguments.

7. Print patients: This will print all of the patients in the waiting list and all
of their attributes. It does not require any input arguments.

8. Print donors: This will print all of the donors waiting for a patient match
and all of their attributes. It does not require any input arguments.

9. Print matches: This will print all of the patient - donor matches that
have been paired but not yet operated on, and the likelihood that the
operation will be a success. It does not require any input arguments.

10. Operate: This will "operate" on a donor - patient match and will
determine whether or not the operation was a success using a random
function and the patient's likelihood of survivability. It does not require any
input arguments.

Functions Implemented :
myTree.buildGraph(); //builds our city graph

myTree.buildDonorList(); //builds our donor table and fills it with
placeholders

myTree.buildPatientList(); //builds our patient table and fills it with
placeholders

myTree.enqueue(newPair); //adds the pair to the surgery waiting list

myTree.countPatients(); //counts the number of patients in the table and
assigns it to a variable

myTree.countDonors(); //counts the number of donors in the table and
assigns it to a variable

myTree.printPatients(); //prints the list of patients and all their attributes

myTree.printDonors(); //prints the list of donors and all their attributes

myTree.printMatches(); //prints the list of matches made (that have not
undergone sugery)

myTree.printOrganQuantity(organ); //prints the list of matches made (that
have not undergone sugery)

myTree.Operate(); //Performs a surgery on the first Pair in the queue

myTree.deletePatient(name); //deletes patient from patient table

myTree.deleteDonor(name); //deletes donor from donor table

Credits : Yash Sancheti, Aditya Kurele
